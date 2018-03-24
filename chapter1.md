# Search and Booking

### Search for nearby clinics

### ![](/assets/Simulator Screen Shot - iPhone SE - 2018-03-18 at 02.24.11.png)

#### Example Query

```
{
  "radius": 400,
  "latitude": 40.758464,
  "longitude": -73.981806,
  "date": "2018-03-01T17:32:45.113Z"
}
```

#### Example Response

```
{
  "success": true,
  "status": 200,
  "result": {
    "clinics": [
      {
        "id": 832,
        "clinicName": "Magic Pts - 34 W 44th St",
        "startBusinessHour": "9:00",
        "endBusinessHour": "18:00",
        "phone": "555-555-5555",
        "fax": "",
        "email": "dan@test.com",
        "about": "I am a manager updating this clinic",
        "isHSSAffiliate": true,
        "hssReviewStatus": null,
        "avatarUrl": null,
        "smallAvatarUrl": null,
        "rating": "5",
        "numberOfReviews": 2,
        "isActive": true,
        "isBasic": false,
        "timeZone": "America/New_York",
        "useClinicName": false,
        "logoUrl": null,
        "smallLogoUrl": null,
        "socialId": null,
        "locationId": 946,
        "companyId": 106,
        "policyId": 174,
        "appointmentTypeId": 155,
        "yelpId": 1146,
        "location": {
          "address": "34 W 44th St",
          "city": "New York",
          "state": "NY",
          "zipcode": "10036",
          "lat": 40.7555348,
          "lng": -73.9817351,
          "geo": {
            "type": "Point",
            "coordinates": [
              -73.9817351,
              40.7555348
            ]
          },
          "formattedAddress": "34 W 44th St, New York, NY 10036, USA",
          "distance": 476.31967548
        },
        "company": {
          "id": 106,
          "companyName": "Magic Pts",
          "email": "test@test.com",
          "phone": "444-444-4444",
          "website": "",
          "avatarUrl": "https://api.dev.betterpt.com/v0/api/companies/106/avatar?size=large",
          "smallAvatarUrl": "https://api.dev.betterpt.com/v0/api/companies/106/avatar?size=small",
          "locationId": 943
        },
        "plans": [],
        "policy": {
          "id": 174,
          "hoursNotice": 45,
          "cancellationFee": 44,
          "details": "test here",
          "createdAt": "2018-03-01T17:32:45.144Z",
          "updatedAt": "2018-03-01T17:32:45.144Z"
        },
        "appointmentType": {
          "id": 155,
          "firstVisitDuration": 55,
          "followUpVisitDuration": 5,
          "createdAt": "2018-03-01T17:32:45.113Z",
          "updatedAt": "2018-03-01T17:32:45.113Z"
        },
        "social": null,
        "yelp": {
          "id": 1146,
          "businessLink": "https://www.yelp.com/biz/spear-physical-therapy-midtown-w-44th-st-manhattan-5?adjust_creative=hxhdUaqvO4TGzEY4K2Kejg&utm_campaign=yelp_api_v3&utm_medium=api_v3_business_lookup&utm_source=hxhdUaqvO4TGzEY4K2Kejg",
          "stars": 4.5,
          "numberOfReviews": 78,
          "lastUpdate": "2018-03-18T05:01:44.000Z",
          "createdAt": "2018-03-01T05:02:00.003Z",
          "updatedAt": "2018-03-18T05:01:44.648Z"
        },
        "availabilities": [
          {
            "start": "2018-03-18",
            "end": "2018-03-18",
            "clinicId": 832,
            "therapistId": 271
          }
        ]
      },
```

### Search Results Display

![](/assets/results1.png)

### Clinic Detail View

![](/assets/clinicdetail.png)

#### Example Query

```
{
  "date": "2018-02-28T21:02:47.453Z"
}
```

#### Example Response

```
{
  "success": true,
  "status": 200,
  "result": {
    "therapists": [
      {
        "accountType": 2,
        "id": 271,
        "isActive": true,
        "role": "self",
        "isTherapist": true,
        "createdAt": "2018-02-28T21:02:47.453Z",
        "updatedAt": "2018-03-08T19:18:05.652Z",
        "therapistId": 271,
        "companyId": 106,
        "user": {
          "uid": "69715a5b-c0e4-4d0b-9183-1d11d6c8c4b3",
          "firstName": "Clara",
          "lastName": "Lopez",
          "email": "daniel+magicsched@betterpt.com",
          "phone": null,
          "gender": "F",
          "birthday": null,
          "timezone": "America/New_York",
          "profileImgUrl": null,
          "smallProfileImgUrl": null,
          "hasLoggedIn": true,
          "createdAt": "2018-02-28T21:02:47.445Z",
          "updatedAt": "2018-03-01T20:57:59.998Z",
          "employeeId": 271
        },
        "therapist": {
          "id": 271,
          "degreeOrCertification": "test",
          "yearsExperience": "1986-10-01T00:00:00.000Z",
          "bio": "teste",
          "createdAt": "2018-03-01T22:48:20.947Z",
          "updatedAt": "2018-03-08T19:18:12.727Z",
          "availabilities": [
            {
              "start": "2018-03-18",
              "end": "2018-03-18",
              "id": 1440261,
              "clinicId": 832,
              "therapistId": 271
            }
          ]
        },
        "clinics": [
          {
            "id": 832,
            "clinicName": "Magic Pts - 34 W 44th St",
            "startBusinessHour": "9:00",
            "endBusinessHour": "18:00",
            "phone": "555-555-5555",
            "fax": "",
            "email": "dan@test.com",
            "about": "I am a manager updating this clinic",
            "isHSSAffiliate": true,
            "hssReviewStatus": null,
            "avatarUrl": null,
            "smallAvatarUrl": null,
            "rating": "5",
            "numberOfReviews": 2,
            "isActive": true,
            "isBasic": false,
            "timeZone": "America/New_York",
            "useClinicName": false,
            "logoUrl": null,
            "smallLogoUrl": null,
            "socialId": null,
            "locationId": 946,
            "companyId": 106,
            "policyId": 174,
            "appointmentTypeId": 155,
            "yelpId": 1146,
            "policy": {
              "id": 174,
              "hoursNotice": 45,
              "cancellationFee": 44,
              "details": "test here",
              "createdAt": "2018-03-01T17:32:45.144Z",
              "updatedAt": "2018-03-01T17:32:45.144Z"
            },
            "appointmentType": {
              "id": 155,
              "firstVisitDuration": 55,
              "followUpVisitDuration": 5,
              "createdAt": "2018-03-01T17:32:45.113Z",
              "updatedAt": "2018-03-01T17:32:45.113Z"
            },
            "clinicEmployee": {
              "createdAt": "2018-03-08T18:16:39.135Z",
              "updatedAt": "2018-03-08T18:16:39.135Z",
              "clinicId": 832,
              "employeeId": 271
            }
          },
          {
            "id": 834,
            "clinicName": "Magic Pts - 14 Western Pkwy",
            "startBusinessHour": "9:00",
            "endBusinessHour": "18:00",
            "phone": "888-888-8888",
            "fax": null,
            "email": "test@test.com",
            "about": null,
            "isHSSAffiliate": true,
            "hssReviewStatus": null,
            "avatarUrl": null,
            "smallAvatarUrl": null,
            "rating": null,
            "numberOfReviews": null,
            "isActive": false,
            "isBasic": false,
            "timeZone": "America/New_York",
            "useClinicName": false,
            "logoUrl": null,
            "smallLogoUrl": null,
            "socialId": null,
            "locationId": 947,
            "companyId": 106,
            "policyId": null,
            "appointmentTypeId": null,
            "yelpId": null,
            "policy": null,
            "appointmentType": null,
            "clinicEmployee": {
              "createdAt": "2018-03-08T18:17:13.556Z",
              "updatedAt": "2018-03-08T18:17:13.556Z",
              "clinicId": 834,
              "employeeId": 271
            }
          },
          {
            "id": 837,
            "clinicName": "new magic upper west",
            "startBusinessHour": "9:00",
            "endBusinessHour": "18:00",
            "phone": "333-333-3333",
            "fax": null,
            "email": "test@test.com",
            "about": "hello clinic",
            "isHSSAffiliate": true,
            "hssReviewStatus": null,
            "avatarUrl": null,
            "smallAvatarUrl": null,
            "rating": null,
            "numberOfReviews": null,
            "isActive": false,
            "isBasic": false,
            "timeZone": "America/New_York",
            "useClinicName": true,
            "logoUrl": null,
            "smallLogoUrl": null,
            "socialId": null,
            "locationId": 949,
            "companyId": 106,
            "policyId": 189,
            "appointmentTypeId": 170,
            "yelpId": null,
            "policy": {
              "id": 189,
              "hoursNotice": 55,
              "cancellationFee": 55,
              "details": "tewst",
              "createdAt": "2018-03-15T21:15:44.210Z",
              "updatedAt": "2018-03-15T21:15:44.210Z"
            },
            "appointmentType": {
              "id": 170,
              "firstVisitDuration": 55,
              "followUpVisitDuration": 55,
              "createdAt": "2018-03-15T21:15:44.283Z",
              "updatedAt": "2018-03-15T21:15:44.283Z"
            },
            "clinicEmployee": {
              "createdAt": "2018-03-08T18:22:32.568Z",
              "updatedAt": "2018-03-08T18:22:32.568Z",
              "clinicId": 837,
              "employeeId": 271
            }
          }
        ],
        "clinicEmployee": {
          "createdAt": "2018-03-08T18:16:39.135Z",
          "updatedAt": "2018-03-08T18:16:39.135Z",
          "clinicId": 832,
          "employeeId": 271
        }
      }
    ]
  }
}
```

### Physical Therapist Results View

![](/assets/pt results.png)

### Physical Therapist Detail View

![](/assets/pt detail.png)

#### Example Query

```
{
  "date": "2018-02-28T21:02:47.453Z",
  clinicId: 61

}
```

#### Example Response

```
{
  "success": true,
  "status": 200,
  "result": {
    "availabilities": [
      {
        "source": "15ec90e7-1da3-11e8-ab59-1b8c3026a27d",
        "start": "2018-03-18T13:15:00-04:00",
        "end": "2018-03-18T14:10:00-04:00",
        "clinicId": 832
      },
      {
        "source": "15ec90e7-1da3-11e8-ab59-1b8c3026a27d",
        "start": "2018-03-18T13:30:00-04:00",
        "end": "2018-03-18T14:25:00-04:00",
        "clinicId": 832
      },
      {
        "source": "15ec90e7-1da3-11e8-ab59-1b8c3026a27d",
        "start": "2018-03-18T13:45:00-04:00",
        "end": "2018-03-18T14:40:00-04:00",
        "clinicId": 832
      },
      {
        "source": "15ec90e7-1da3-11e8-ab59-1b8c3026a27d",
        "start": "2018-03-18T14:00:00-04:00",
        "end": "2018-03-18T14:55:00-04:00",
        "clinicId": 832
      }
  ]
}
```

### Condition Detail View

![](/assets/condition booking.png)

### Booking Confirmation

![](/assets/confirm booking.png)

#### Example Parameters

```
{
  "isFollowupAppointment": true,
  "caseId": 51,
  "startTime": "2018-02-28T21:02:47.453Z"
}
```

#### Example Response

```
{
  "success" : true,
  "status" : 201,
  "result" : {
    "status" : "booked",
    "caseId" : 530,
    "duration" : 5,
    "case" : {
      "patientId" : 99,
      "id" : 530,
      "referredBy" : "Dr. FeelMe",
      "description" : "Hurts",
      "updatedAt" : "2017-12-01T23:16:34.142Z",
      "createdAt" : "2017-12-01T23:16:34.142Z"
    },
    "formattedAddress" : null,
    "employeeIdWhoCancelled" : null,
    "endTime" : "2018-03-18T17:35:00.000Z",
    "isReviewed" : false,
    "companyId" : 106,
    "cancelledBy" : null,
    "createdAt" : "2018-03-18T16:06:08.297Z",
    "noteId" : null,
    "updatedAt" : "2018-03-18T16:06:08.297Z",
    "id" : 1095,
    "timeZone" : "America\/New_York",
    "patientId" : 99,
    "clinicId" : 832,
    "fee" : 0,
    "note" : null,
    "startTime" : "2018-03-18T17:30:00.000Z",
    "employeeTherapistId" : 271
  }
}
```



