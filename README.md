# Hotel-booking-demand
Have you ever wondered when the best time of year to book a hotel room is? Or the optimal length of stay in order to get the best daily rate? What if you wanted to predict whether or not a hotel was likely to receive a disproportionately high number of special requests? 

This hotel booking dataset can help you explore those questions!

I used the dataset and description above from here: https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand. Thanks to those who provide such data for free, beginners need the opportunity to learn from quality data :)

## Data details
1. **hotel** - City Hotel/Resort Hotel. Hotel type: Resort or city.
2. **is_canceled** - A value indicating whether the booking was canceled (1) or not (0).
3. **lead_time** - The number of days elapsed between the date the booking was entered in PMS and the date of arrival.
4. **arrival_date_year** - year of arrival.
5. **arrival_date_month** - month of arrival.
6. **arrival_date_week_number** - Week number of the year of arrival date.
7. **arrival_date_day_of_month** - Day of arrival.
8. **stays_in_weekend_nights** - The number of weekend nights (Saturday or Sunday) that the guest stayed or booked at the hotel.
9. **stays_in_week_nights** - The number of nights per week (Monday to Friday) that the guest stayed or booked at the hotel.
10. **adults** - Number of adults.
11. **children** - Number of children.
12. **babies** - Number of babies.
13. **meal** - Type of meal booked. Categories are presented in standard food packages:
    1. Undefined / SC - no power pack;
    2. BB - bed and breakfast;
    3. HB - half board (breakfast and one meal - usually dinner);
    4. FB - Full board (breakfast, lunch and dinner)
14. **country** - Country of origin. Categories are presented in ISO 3155–3:2013 format.
15. **market_segment** - Designation of the market segment. In the categories, the term "TA" stands for "Travel Agents" and "TO" stands for "Travel Operators".
16. **distribution_channel** - Reservation distribution channel. The term "TA" means "Travel Agents" and "TO" means "Tour Operators".
17. **is_repeated_guest** - A value indicating whether the booking name was from a repeat guest (1) or not (0).
18. **previous_cancellations** - The number of previous bookings that were canceled by the client prior to the current booking.
19. **previous_bookings_not_canceled** - The number of previous bookings not canceled by the client prior to the current booking.
20. **reserved_room_type** - The room type code is reserved. The code is presented instead of a notation for reasons of anonymity.
21. **assigned_room_type** - Code of the room type assigned to the booking. Sometimes the assigned room type differs from the booked type for reasons related to the operation of the hotel (for example, overbooking) or at the request of the client. The code is presented instead of a notation for reasons of anonymity.
22. **booking_changes** - The number of changes/amendments made to the booking from the time the booking was entered into PMS until check-in or cancellation.
23. **deposit_type** - An indication of whether the customer made a deposit to secure the booking. This variable can take three categories: No Deposit - no deposit was made; Non Refund - a deposit in the amount of the full cost of living has been paid; Refundable - a deposit was made in the amount of the total cost of living.
24. **agent** - Identifier of the travel agency that made the booking.
25. **company** - Identifier of the company/organization that made the booking or is responsible for paying for the booking. An identifier is presented instead of a designation for reasons of anonymity
26. **days_in_waiting_list** - The number of days the booking was on the waiting list before it was confirmed to the client.
27. **customer_type** - Reservation type, one of four categories:
    1. Contract - when the booking is associated with an allotment or other type of contract;
    2. Group - when the booking is associated with a group;
    3. Transient - when the booking is not part of a group or contract and is not linked to another temporary booking;
    4. Transient-party - when the booking is temporary, but is associated with at least another temporary booking.
28. **adr** - Average daily rate, determined by dividing the sum of all accommodation transactions by the total number of nights of stay.
29. **required_car_parking_spaces** - The number of parking spaces required by the customer.
30. **total_of_special_requests** - The number of special requests the client has (for example, two single beds or an upper floor.
31. **reservation_status** - The status of the last reservation, allowing one of three categories:
    1. Canceled - the booking was canceled by the client;
    2. Check-Out - the client has registered, but has already left;
    3. No-Show - the client did not check in and did not report the reason why the hotel
32. **reservation_status_date** - Date when the last status was set. This variable can be used in conjunction with ReservationStatus to understand when a booking was canceled or when a customer checked out of a hotel.

# Спрос на бронирование отелей
Вы когда-нибудь задумывались, в какое время года лучше всего бронировать номер в отеле? Или оптимальную продолжительность пребывания, чтобы получить лучший дневной тариф? Что, если вы хотите предсказать, получит ли отель непропорционально большое количество специальных запросов?

Этот датасет о бронировании отелей поможет вам разобраться в этих вопросах!

Использовал датасет и описание выше отсюда: https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand. Благодарю тех, кто предоставляет такие данные бесплатно, новичкам нужна возможность учиться на хороших данных :)  

## Сведения о данных
1. **hotel** - City Hotel/Resort Hotel. Вид отеля: Курортный или городской.  
2. **is_canceled** - Значение, указывающее, было ли бронирование отменено (1) или нет (0).  
3. **lead_time** - Количество дней, прошедших между датой ввода бронирования в PMS и датой прибытия.  
4. **arrival_date_year** - год прибытия.  
5. **arrival_date_month** - месяц прибытия.  
6. **arrival_date_week_number** - Номер недели года даты прибытия.  
7. **arrival_date_day_of_month** - День прибытия.  
8. **stays_in_weekend_nights** - Количество ночей в выходные дни (суббота или воскресенье), в течение которых гость останавливался или забронировал проживание в отеле.  
9. **stays_in_week_nights** - Количество ночей в неделю (с понедельника по пятницу), в течение которых гость останавливался или забронировал проживание в отеле.  
10. **adults** - Количество взрослых.  
11. **children** - Количество детей.  
12. **babies** - Количество младенцев.  
13. **meal** - Тип забронированного питания. Категории представлены в стандартных пакетах питания:  
    1. Undefined/SC – без пакета питания;  
    2. ВВ – кровать и завтрак;  
    3. HB – полупансион (завтрак и один прием пищи – обычно ужин);  
    4. FB – Полный пансион (завтрак, обед и ужин)
14. **country** - Страна происхождения. Категории представлены в формате ISO 3155–3:2013.
15. **market_segment** - Обозначение сегмента рынка. В категориях термин «TA» означает «Туристические агенты», а «TO» означает «Туристические операторы».  
16. **distribution_channel** - Канал распространения бронирования. Термин «ТА» означает «Туристические агенты», а «ТО» означает «Туристические операторы».  
17. **is_repeated_guest** - Значение, указывающее, было ли имя бронирования от повторного гостя (1) или нет (0).  
18. **previous_cancellations** - Количество предыдущих бронирований, которые были отменены клиентом до текущего бронирования.  
19. **previous_bookings_not_canceled** - Количество предыдущих бронирований, не отмененных клиентом до текущего бронирования.  
20. **reserved_room_type** - Код типа номера зарезервирован.  Код представлен вместо обозначения из соображений анонимности.  
21. **assigned_room_type** - Код типа номера, присвоенного бронированию.  Иногда присвоенный тип номера отличается от забронированного типа по причинам, связанным с работой отеля (например, избыточное бронирование) или по желанию клиента.  Код представлен вместо обозначения из соображений анонимности. 
22. **booking_changes** - Количество изменений/поправок, внесенных в бронирование с момента ввода бронирования в PMS до момента заселения или отмены.  
23. **deposit_type** - Указание на то, внес ли клиент депозит для гарантии бронирования.  Эта переменная может принимать три категории: No Deposit – депозит не вносился;  Non Refund – внесен залог в размере полной стоимости проживания;  Возвратный – был внесен депозит в размере под общую стоимость проживания.  
24. **agent** - Идентификатор туристического агентства, оформившего бронирование.  
25. **company** - Идентификатор компании/организации, оформившей бронирование или ответственной за оплату бронирования. Идентификатор представлен вместо обозначения из соображений анонимности
26. **days_in_waiting_list** - Количество дней, в течение которых бронирование находилось в списке ожидания, прежде чем оно было подтверждено клиенту.  
27. **customer_type** - Тип бронирования, предполагающий одну из четырех категорий: 
    1. Contract — когда бронирование связано с выделением или другим типом контракта;  
    2. Group — когда бронирование связано с группой;  
    3. Transient — когда бронирование не является частью группы или контракта и не связано с другим временным бронированием;  
    4. Transient-party — когда бронирование является временным, но связано как минимум с другим временным бронированием.
28. **adr** - Средняя дневная ставка, определяемая путем деления суммы всех транзакций по размещению на общее количество ночей проживания.  
29. **required_car_parking_spaces** - Требуемое заказчиком количество парковочных мест.  
30. **total_of_special_requests** - Количество особых пожеланий клиента (например, две односпальные кровати или верхний этаж. 
31. **reservation_status** - Статус последнего бронирования, допускающий одну из трех категорий: 
    1. Canceled – бронирование было отменено клиентом;  
    2. Check-Out – клиент зарегистрировался, но уже ушел;  
    3. No-Show – клиент не зарегистрировался и не сообщил о причине, по которой отель
32. **reservation_status_date** - Дата, когда был установлен последний статус.  Эту переменную можно использовать в сочетании с ReservationStatus, чтобы понять, когда было отменено бронирование или когда клиент выписался из отеля.
