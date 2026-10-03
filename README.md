# LAB-02-Car-share-Store-Map
#

## 1. 2D Story Map

```mermaid
flowchart LR

    A["ACCOUNT MANAGEMENT<br/><br/>Register<br/>Login<br/>Verify Identity"]

    B["FIND A CAR<br/><br/>Search Available Cars<br/>View Car Details<br/>Filter Cars"]

    C["BOOK A CAR<br/><br/>Select Car<br/>Select Date/Time<br/>Confirm Booking"]

    D["PICK UP CAR<br/><br/>View Pickup Location<br/>Unlock Car<br/>Start Rental"]

    E["USE CAR<br/><br/>Start Trip<br/>View Trip Details<br/>Track Trip"]

    F["RETURN CAR<br/><br/>End Trip<br/>Lock Car<br/>Confirm Return"]

    G["PAYMENT<br/><br/>Calculate Cost<br/>Make Payment<br/>View Receipt"]

    A --> B --> C --> D --> E --> F --> G
```

## 2. Walking Skeleton MVP

The Walking Skeleton represents the smallest end-to-end version of the
peer-to-peer car-sharing application.

### MVP User Journey

Register/Login  
↓  
Search Available Car  
↓  
View Car  
↓  
Book Car  
↓  
Pick Up Car  
↓  
Use Car  
↓  
Return Car  
↓  
Make Payment

## 3. MVP Features

- User registration and login
- Search available cars
- View car details
- Select a car
- Select date and time
- Confirm booking
- View pickup location
- Start rental
- End rental
- Calculate rental cost
- Make payment

## 4. Future Features

- Advanced car filters
- Ratings and reviews
- Notifications
- Favourite cars
- Trip history
- Promotional codes
- Referral system
- Advanced GPS tracking
- Insurance options
