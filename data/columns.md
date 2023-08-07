## Column Names and Descriptions for King County Data Set
* `adr` - (Integer) Numeric Average Daily Rate Calculated by dividing the sum of all lodging transactions by the total number of staying nights.
* `adults` -  (Integer) Number of adults
* `agent` - (Integer) ID of the travel agency that made the booking.
* `arrival_date_day_of_month` - (Integer) Day of the month of the arrival date .
* `arrival_date_month` - (Categorical) Month of arrival date with 12 categories: “January” to “December”
* `arrival_date_week_number` - (Integer) Week number of the arrival date
* `arrival_date_year` - (Integer) Year of arrival date 
* `assigned_room_type` - (Categorical) Code for the type of room assigned to the booking. Sometimes the assigned room type differs from the reserved room type due to hotel operation reasons (e.g.overbooking) or by customer request.
* `babies` - (Interger) Number of babies 
* `booking_changes` - (Integer) Number of changes/amendments made to the booking from the moment the booking was entered on the PMS until the moment of check-in or cancellation.
* `children` - (Integer) Number of children 
* `company` - (Categorical) ID of the company/entity that made the booking or responsible for paying the booking.
* `country` -  (Categorical) Country of origin. Categories are represented in the ISO 3155–3:2013 format
* `customer_type` - (Categorical) Type of booking, assuming one of four categories:
    - Contract - when the booking has an allotment or other type of contract associated to it;
    - Group – when the booking is associated to a group;
    - Transient – when the booking is not part of a group or contract, and is not associated to other transient booking;
    - Transient-party – when the booking is transient, but is associated to at least other transient booking.
* `days_inWaiting_list` - (Integer) Number of days the booking was in the
waiting list before it was confirmed to the customer. Calculated by subtracting the date the booking was confirmed to the
customer from the date the booking entered on the PMS.
* `deposit_type` - (Categorical) Indication on if the customer made a
deposit to guarantee the booking. Value calculated based on
the payments identified for the booking in the transaction table before the booking's arrival or cancellation date. This variable can assume three categories: 
    - No Deposit – no deposit was made; In case no payments were found the value is “No Deposit”.
    - Non Refund – a deposit was made in the value of the total stay cost; If the payment was equal or exceeded the total cost of stay, the value is set as “Non Refund”.
    - Refundable – a deposit was made with a value under the total cost of stay; Otherwise the value is set as “Refundable”.
* `distribution_channel` - (Categorical) Booking distribution channel. The term “TA” means “Travel Agents” and “TO” means “Tour Operators”
* `is_canceled` - (Categorical) Value indicating if the booking was canceled (1) or not (0)
* `is_repeated_guest` - (Categorical) Value indicating if the booking name was from a repeated guest (1) or not (0). Variable created by verifying if a profile was associated with the booking customer. If so, and if the customer profile creation date was prior to the creation date for the booking on the PMS database it was assumed the booking was from a repeated guest.
* `lead_time` - (Integer) Number of days that elapsed between the entering date of the booking into the PMS and the arrival date. Subtraction of the entering date from the arrival date.
* `market_segment`- (Categorical) Market segment designation. In categories, the term “TA” means “Travel Agents” and “TO” means “Tour Operators”
* `meal` - (Categorical) Type of meal booked. Categories are presented in standard hospitality meal packages:
    - Undefined/SC – no meal package;
    - BB – Bed & Breakfast;
    - HB – Half board (breakfast and one
    - other meal – usually dinner);
    - FB – Full board (breakfast, lunch and dinner)
* `previous_bookings_not_canceled` - (Integer) Number of previous bookings not cancelled by the customer prior to the current booking. In case there was no customer profile associated with the booking, the value is set to 0. Otherwise, the value is the number of bookings with the same customer profile created before the current booking and not canceled.
* `previous_cancellations` - (Integer) Number of previous bookings that were cancelled by the customer prior to the current booking  In case there was no customer profile associated with the booking, the value is set to 0. Otherwise, the value is the number of bookings with the same customer profile created before the current booking and canceled.
* `required_card_parking_spaces` - (Integer) Number of car parking spaces required by the customer.
* `reservation_status` - (Categorical) Reservation last status, assuming one of three categories:
    - Canceled – booking was canceled by the customer;
    - Check-Out – customer has checked in but already departed;
    - No-Show – customer did not check-in and did inform the hotel of the reason why
* `reservation_status_date` - (Date) Date at which the last status was set. This variable can be used in conjunction with the ReservationStatus to understand when was the booking canceled or when did the customer checked-out of the hotel
* `reserved_room_type` - (Categorical) Code of room type reserved. Code is presented instead of designation for anonymity reasons
* `stays_in_weekend_nights` - (Integer) Number of weekend nights(Saturday or Sunday) the guest stayed or booked to stay at the hotel. Calculated by counting the number of weekend nights from the total number of nights.
* `stays_in_week_nights` - (Integer) Number of week nights (Monday to Friday) the guest stayed or booked to stay at the hotel. Calculated by counting the number of week nights from the total number of nights.
* `total_of_special_requests` - (Integer) Number of special requests made by the customer (e.g. twin bed or high floor)