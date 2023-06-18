Bookmyshow

Actors:

1. User- sequence of operations by end user
    - Login/registration
    - search prefered movie/event based on language ot others
    - select date&time , select seats
    - apply if any offers available
    - complete payment and book tickets
    - print ticket
    - cancel/reschdule movie/event
    - can share ticket details to others
    - can give feedback on movies/events/location
    - can interest on movie/event
    - can set to get notified for preferred movie update
    - can search movie details 
    - can mark upcoming movies 

2. Operator- authorized person from theatre booking counter
    - login
    - can have access to working event/theatre only
    - select movie and book tickets without payment 

3. Admin- theatre/event owners. 
    - login
    - update new/scheduled movies/events with time to bookmyshow
    - notify system on update to proceed
    - cancel/reschedule events

4. System - 
    - show near by theatres first to users
    - calcualte total price and send to user
    - manage booking, (handle concurrent bookings)
    - manage payments (adding/deleting/updating payments)
    - send notifications to users on booked tickets with date, location
    - send notifications on upcoming releases & any offers
    - send notifications on offers to users
    - managing offers
    - Manage advertisement and promotions
    - manage feeback


SOLID principles

    1. handling payment methods(CRUD) - Dependency Inversion
    2. User roles for different logins - Liskov Substitution Principle


Factory design pattern

    1. Login manager
        -handle different types of user
    2. Event manager
        -Movie Manager
            - Movier
        -Other Event Manager
            -Other events

Observer design pattern
    1. Notification manager
        -subscribe for notification
        -unscrubscribe for notification
        -send notification on time remainders/notifications
    2. Advertisement Manager
        -send upcoming events/movies to user

