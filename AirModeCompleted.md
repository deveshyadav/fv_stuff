
Create Shopment:- 627f01d3-61e0-48f5-9b51-fb08be1ab787
Request:- 
{
    "carrier": {
        "scac": "TEST",
        "fvCarrierId": "FV0834338A"
    },
    "customer": {
        "fvCustomerId": "FV3221778A"
    },
    "shipmentIdentification": {
        "shipmentId": "{{shipment_id}}",
        "proNumber": "AIR-PRONUM"
    },
    "stops": [
        {
            "stopSequence": 1,
            "stopType": "load",
            "stopRole": "ship_from",
            "earlyArrival": "{{origin_early_pickup}}",
            "lateArrival": "{{origin_late_pickup}}",
            "location": {
                "name": "Dallas/Fort Worth Airport",
                "address1": "2400 Aviation Dr.",
                "city": "Dallas",
                "state": "TX",
                "postalCode": "75261",
                "country": "US",
                "locationId": {
                    "value": "DFW"
                }
            }
        },
        {
            "stopSequence": 2,
            "stopType": "unload",
            "stopRole": "ship_to",
            "earlyArrival": "{{destination_early_delivery}}",
            "lateArrival": "{{destination_late_delivery}}",
            "location": {
                "name": "Detroit Metro Airport",
                "address1": "198 William Rogell Dr.",
                "city": "Detroit",
                "state": "MI",
                "postalCode": "48242",
                "country": "US",
                "locationId": {
                    "value": "DTW"
                }
            }
        }
    ],
    "shipmentReferences": [
        {
            "qualifier": "mode",
            "value": "air"
        },
        {
            "qualifier": "route_id",
            "value": "AIR-ROUTE"
        },
        {
            "qualifier": "order_number",
            "value": "{{order_number}}"
        },
        {
            "qualifier": "part",
            "value": "AIR-PART1 (50)"
        },
        {
            "qualifier": "part",
            "value": "AIR-PART2 (100)"
        }
    ]
}

Response:-
{
    "shipment": {
        "id": 39812323,
        "fv_id": "FV5849643A",
        "created_by_user_id": null,
        "created_by_org_id": 1004,
        "creator_shipment_id": "AKYUQTTGVG3",
        "driver_id": null,
        "total_distance": 986.6128293179373,
        "progress": null,
        "status_updated_at": null,
        "obc_asset_id": null,
        "trailer_number": null,
        "asset_unqueryable": null,
        "asset_tracking_start_stop": null,
        "created_at": null,
        "updated_at": null,
        "is_accepted": true,
        "is_completed": false,
        "is_integration": true,
        "current_status": null,
        "eta": null,
        "frozen_eta": null,
        "frozen_eta_reason": null,
        "current_exception": null,
        "remaining_distance": null,
        "message_id": null,
        "is_behind_schedule": false,
        "carrier_organization_id": 1003,
        "origin_location_id": null,
        "destination_location_id": null,
        "origin_pickup_window": [
            1731274200.0,
            1731281400.0
        ],
        "destination_delivery_window": [
            1731292200.0,
            1731299400.0
        ],
        "picked_up_at": null,
        "delivered_at": null,
        "mode_id": 7,
        "destination_newloc_id": 288523,
        "origin_newloc_id": 288522,
        "active_until": null,
        "active_status": null,
        "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
        "actor_type": "system",
        "actor_email": "test@freightverify-api.com",
        "is_rack_return": null,
        "pro_number": "AIR-PRONUM",
        "tracking_window": null,
        "rail_creator_shipment_id": "AKYUQTTGVG3",
        "shipment_id_3pl": null,
        "tracking_disabled": null,
        "rail_asset_id": null,
        "route_number": "AIR-ROUTE",
        "trip_plan_number": null,
        "leg": false,
        "vins_added": null,
        "line_of_business_id": 2,
        "submode_id": null,
        "parent_shipment_id": null,
        "status_details": null,
        "current_road_organization_id": null,
        "rail_train_id": null,
        "rail_loaded_status": null,
        "change_details": null,
        "original_schedule_start_day": null,
        "current_schedule_offset": null,
        "allow_origin_window_carrier_update": null,
        "allow_destination_window_carrier_update": null,
        "trip_plan_id": null,
        "shipment_details": {
            "hasParts": true
        },
        "shipment_stops": [
            {
                "id": 288481213,
                "shipment_id": 39812323,
                "stop_sequence": 1,
                "org_location_id": null,
                "is_missed": false,
                "earliest_arrival_datetime": "2024-11-10T21:30:00+00:00",
                "latest_arrival_datetime": "2024-11-10T23:30:00+00:00",
                "created_at": "2024-11-11T04:56:49.080687+00:00",
                "updated_at": null,
                "stop_reason": "LD",
                "stop_role": "SF",
                "eta": null,
                "frozen_eta": null,
                "frozen_eta_reason": null,
                "is_behind_schedule": false,
                "distance": 0.0,
                "remaining_distance": null,
                "arrival_ping": 0,
                "is_relay_stop": false,
                "obc_asset_id": null,
                "creator_location_id": "DFW",
                "arrived_at": null,
                "departed_at": null,
                "location_id": 288522,
                "stop_identifier": "",
                "mode_id": 7,
                "child_shipment_id": null,
                "geofence_entered": null,
                "is_fv_eta": null,
                "change_details": null,
                "geofence_details": null
            },
            {
                "id": 288481214,
                "shipment_id": 39812323,
                "stop_sequence": 2,
                "org_location_id": null,
                "is_missed": false,
                "earliest_arrival_datetime": "2024-11-11T02:30:00+00:00",
                "latest_arrival_datetime": "2024-11-11T04:30:00+00:00",
                "created_at": "2024-11-11T04:56:49.080687+00:00",
                "updated_at": null,
                "stop_reason": "UL",
                "stop_role": "ST",
                "eta": null,
                "frozen_eta": null,
                "frozen_eta_reason": null,
                "is_behind_schedule": false,
                "distance": 0.0,
                "remaining_distance": null,
                "arrival_ping": 0,
                "is_relay_stop": false,
                "obc_asset_id": null,
                "creator_location_id": "DTW",
                "arrived_at": null,
                "departed_at": null,
                "location_id": 288523,
                "stop_identifier": "",
                "mode_id": 7,
                "child_shipment_id": null,
                "geofence_entered": null,
                "is_fv_eta": null,
                "change_details": null,
                "geofence_details": null
            }
        ]
    }
}



Asset Assignment:- fc89e29c-f516-4548-98d0-e716e720b479
Request:-
{
    "carrier": {
        "scac": "TEST",
        "fvCarrierId": "FV0834338A"
    },
    "telematics": {
        "trackingAssetId": "AIR-ASSET"
    },
    "eventDetail": {
        "eventDate": "{{origin_early_pickup}}",
        "event": "XB"
    }
}

Response:-
{
    "shipment_status": {
        "id": 3255223075,
        "organization_id": 1003,
        "user_id": null,
        "shipment_id": 39812323,
        "shipment_stop_id": null,
        "status_location_id": null,
        "actual_created_at": "2024-11-10T21:30:00+00:00",
        "remarks": "Assign asset",
        "created_at": null,
        "updated_at": null,
        "obc_asset_id": "AIR-ASSET",
        "driver_id": null,
        "status_code": "XB",
        "status_reason_code": null,
        "is_exception": false,
        "status_type": 1,
        "message_id": null,
        "longitude": null,
        "latitude": null,
        "processed_at": "2024-11-11T05:03:24.298253+00:00",
        "trailer_number": null,
        "status_details": "{}",
        "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
        "actor_type": "system",
        "actor_email": "test@freightverify-api.com",
        "rail_asset_id": null,
        "equipment_desc": null
    }
}


Position Event- At Dallas :- 2c331bc4-4b05-49d0-a0ef-22f311b234d0

Request:-
{
    "carrier": {
        "scac": "TEST",
        "fvCarrierId": "FV0834338A"
    },
    "location": {
        "latitude": 32.898,
        "longitude": -97.04
    },
    "eventDetail": {
        "eventDate": "{{origin_actual_pickup}}",
        "event": "LO"
    }
}

Response:-
{
    "shipment_status": {
        "id": 3255223076,
        "organization_id": 1003,
        "user_id": null,
        "shipment_id": 39812323,
        "shipment_stop_id": null,
        "status_location_id": null,
        "actual_created_at": "2024-11-10T22:30:00+00:00",
        "remarks": null,
        "created_at": null,
        "updated_at": null,
        "obc_asset_id": null,
        "driver_id": null,
        "status_code": "LO",
        "status_reason_code": null,
        "is_exception": false,
        "status_type": 1,
        "message_id": null,
        "longitude": -97.04,
        "latitude": 32.898,
        "processed_at": "2024-11-11 05:05:03.906190+00:00",
        "trailer_number": null,
        "status_details": "{\"last_reported_at\": null, \"current_latitude\": 32.898, \"current_longitude\": -97.04, \"current_city\": \"Dallas\", \"current_state\": \"TX\", \"current_postal_code\": \"75261\", \"current_country\": \"US\", \"status_code\": \"LO\", \"reported_at\": \"2024-11-10T22:30:00Z\", \"reported_at_local\": \"2024-11-10 16:30:00\", \"created_at\": \"2024-11-11T05:04:54.057366Z\"}",
        "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
        "actor_type": "system",
        "actor_email": "test@freightverify-api.com",
        "rail_asset_id": null,
        "equipment_desc": null
    }
}


Carrier Departure from Origin Dallas:- c6b249d7-981a-4697-8661-9c958b0ec4c5

Request:-
{
    "carrier": {
        "scac": "TEST",
        "fvCarrierId": "FV0834338A"
    },
    "stopSequence": 1,
    "eventDetail": {
        "eventDate": "{{origin_actual_pickup}}",
        "event": "X3",
        "reason": "NS"
    }
}

Response:-
{
    "shipment_status": {
        "id": 3255223079,
        "organization_id": 1003,
        "user_id": null,
        "shipment_id": 39812323,
        "shipment_stop_id": 288481213,
        "status_location_id": null,
        "actual_created_at": "2024-11-10T22:30:00+00:00",
        "remarks": null,
        "created_at": null,
        "updated_at": null,
        "obc_asset_id": null,
        "driver_id": null,
        "status_code": "X3",
        "status_reason_code": "NS",
        "is_exception": false,
        "status_type": 1,
        "message_id": null,
        "longitude": null,
        "latitude": null,
        "processed_at": "2024-11-11 05:30:39.821920+00:00",
        "trailer_number": null,
        "status_details": "{\"last_reported_at\": \"2024-11-10T22:30:00Z\", \"current_latitude\": 32.898, \"current_longitude\": -97.04, \"current_city\": \"Dallas\", \"current_state\": \"TX\", \"current_postal_code\": \"75261\", \"current_country\": \"US\", \"status_code\": \"X3\", \"reported_at\": \"2024-11-10T22:30:00Z\", \"reported_at_local\": \"2024-11-10 16:30:00\", \"created_at\": \"2024-11-11T05:30:39.669175Z\"}",
        "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
        "actor_type": "system",
        "actor_email": "test@freightverify-api.com",
        "rail_asset_id": null,
        "equipment_desc": null
    }
}


Location event-Departing Dallas:- 9ef74539-3854-46cc-a7a5-55964362dff5
Request:-
{
    "carrier": {
        "scac": "TEST",
        "fvCarrierId": "FV0834338A"
    },
    "location": {
        "latitude": 33.028737,
        "longitude": -96.755493
    },
    "eventDetail": {
        "eventDate": "{{origin_actual_departure}}",
        "event": "LO"
    }
}

Response:-
{
    "shipment_status": {
        "id": 3255223080,
        "organization_id": 1003,
        "user_id": null,
        "shipment_id": 39812323,
        "shipment_stop_id": null,
        "status_location_id": null,
        "actual_created_at": "2024-11-10T23:30:00+00:00",
        "remarks": null,
        "created_at": null,
        "updated_at": null,
        "obc_asset_id": null,
        "driver_id": null,
        "status_code": "LO",
        "status_reason_code": null,
        "is_exception": false,
        "status_type": 1,
        "message_id": null,
        "longitude": -96.755493,
        "latitude": 33.028737,
        "processed_at": "2024-11-11 05:32:54.247391+00:00",
        "trailer_number": null,
        "status_details": "{\"last_reported_at\": \"2024-11-10T22:30:00Z\", \"current_latitude\": 33.028737, \"current_longitude\": -96.755493, \"current_city\": \"Plano\", \"current_state\": \"TX\", \"current_postal_code\": \"75075\", \"current_country\": \"US\", \"status_code\": \"LO\", \"reported_at\": \"2024-11-10T23:30:00Z\", \"reported_at_local\": \"2024-11-10 17:30:00\", \"created_at\": \"2024-11-11T05:32:47.748499Z\"}",
        "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
        "actor_type": "system",
        "actor_email": "test@freightverify-api.com",
        "rail_asset_id": null,
        "equipment_desc": null
    }
}


Carrier Departing Event-Dallas:- 47b9d95d-e952-4824-9b95-7c11a58d50a8

Request:-
{
    "carrier": {
        "scac": "TEST",
        "fvCarrierId": "FV0834338A"
    },
    "stopSequence": 1,
    "eventDetail": {
        "eventDate": "{{origin_actual_departure}}",
        "event": "AF",
        "reason": "NS"
    }
}

Resposne:-
{
    "shipment_status": {
        "id": 3255223083,
        "organization_id": 1003,
        "user_id": null,
        "shipment_id": 39812323,
        "shipment_stop_id": 288481213,
        "status_location_id": null,
        "actual_created_at": "2024-11-10T23:30:00+00:00",
        "remarks": null,
        "created_at": null,
        "updated_at": null,
        "obc_asset_id": null,
        "driver_id": null,
        "status_code": "AF",
        "status_reason_code": "NS",
        "is_exception": false,
        "status_type": 1,
        "message_id": null,
        "longitude": null,
        "latitude": null,
        "processed_at": "2024-11-11 05:39:09.364373+00:00",
        "trailer_number": null,
        "status_details": "{\"last_reported_at\": \"2024-11-10T23:30:00Z\", \"current_latitude\": 33.028737, \"current_longitude\": -96.755493, \"current_city\": \"Plano\", \"current_state\": \"TX\", \"current_postal_code\": \"75075\", \"current_country\": \"US\", \"status_code\": \"AF\", \"reported_at\": \"2024-11-10T23:30:00Z\", \"reported_at_local\": \"2024-11-10 17:30:00\", \"created_at\": \"2024-11-11T05:39:09.208406Z\"}",
        "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
        "actor_type": "system",
        "actor_email": "test@freightverify-api.com",
        "rail_asset_id": null,
        "equipment_desc": null
    }
}

Location Event-Arkasansas :- 1c4404ce-c57a-448e-8903-43cc74ebb852
Request:-
{
    "carrier": {
        "scac": "TEST",
        "fvCarrierId": "FV0834338A"
    },
    "location": {
        "latitude": 36.42829,
        "longitude": -91.541714
    },
    "eventDetail": {
        "eventDate": "{{onroute_arkansas}}",
        "event": "LO"
    }
}
Response:-
{
    "shipment_status": {
        "id": 3255223084,
        "organization_id": 1003,
        "user_id": null,
        "shipment_id": 39812323,
        "shipment_stop_id": null,
        "status_location_id": null,
        "actual_created_at": "2024-11-11T00:30:00+00:00",
        "remarks": null,
        "created_at": null,
        "updated_at": null,
        "obc_asset_id": null,
        "driver_id": null,
        "status_code": "LO",
        "status_reason_code": null,
        "is_exception": false,
        "status_type": 1,
        "message_id": null,
        "longitude": -91.541714,
        "latitude": 36.42829,
        "processed_at": "2024-11-11 05:40:43.943517+00:00",
        "trailer_number": null,
        "status_details": "{\"last_reported_at\": \"2024-11-10T23:30:00Z\", \"current_latitude\": 36.42829, \"current_longitude\": -91.541714, \"current_city\": \"Mammoth Spring\", \"current_state\": \"AR\", \"current_postal_code\": \"72554\", \"current_country\": \"US\", \"status_code\": \"LO\", \"reported_at\": \"2024-11-11T00:30:00Z\", \"reported_at_local\": \"2024-11-10 18:30:00\", \"created_at\": \"2024-11-11T05:40:38.428393Z\"}",
        "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
        "actor_type": "system",
        "actor_email": "test@freightverify-api.com",
        "rail_asset_id": null,
        "equipment_desc": null
    }
}

  Location Event-Indiana:- 50080649-1c70-441a-9ed9-84a338f0b3e5
Request:-
{
    "carrier": {
        "scac": "TEST",
        "fvCarrierId": "FV0834338A"
    },
    "location": {
        "latitude": 39.777948,
        "longitude": -86.817086
    },
    "eventDetail": {
        "eventDate": "{{onroute_indiana}}",
        "event": "LO"
    }
}
Response:-
{
    "shipment_status": {
        "id": 3255223085,
        "organization_id": 1003,
        "user_id": null,
        "shipment_id": 39812323,
        "shipment_stop_id": null,
        "status_location_id": null,
        "actual_created_at": "2024-11-11T01:30:00+00:00",
        "remarks": null,
        "created_at": null,
        "updated_at": null,
        "obc_asset_id": null,
        "driver_id": null,
        "status_code": "LO",
        "status_reason_code": null,
        "is_exception": false,
        "status_type": 1,
        "message_id": null,
        "longitude": -86.817086,
        "latitude": 39.777948,
        "processed_at": "2024-11-11 05:43:27.174200+00:00",
        "trailer_number": null,
        "status_details": "{\"last_reported_at\": \"2024-11-11T00:30:00Z\", \"current_latitude\": 39.777948, \"current_longitude\": -86.817086, \"current_city\": \"Bainbridge\", \"current_state\": \"IN\", \"current_postal_code\": \"46105\", \"current_country\": \"US\", \"status_code\": \"LO\", \"reported_at\": \"2024-11-11T01:30:00Z\", \"reported_at_local\": \"2024-11-10 20:30:00\", \"created_at\": \"2024-11-11T05:43:26.200796Z\"}",
        "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
        "actor_type": "system",
        "actor_email": "test@freightverify-api.com",
        "rail_asset_id": null,
        "equipment_desc": null
    }
}


Position Event-Approaching Detroit dest:-248046b1-6e74-4f56-b828-3a7c6f4874ff
Request:-
{
    "carrier": {
        "scac": "TEST",
        "fvCarrierId": "FV0834338A"
    },
    "location": {
        "latitude": 42.004097,
        "longitude": -83.587433
    },
    "eventDetail": {
        "eventDate": "{{destination_actual_approach}}",
        "event": "LO"
    }
}

Response:-
{
    "shipment_status": {
        "id": 3255223086,
        "organization_id": 1003,
        "user_id": null,
        "shipment_id": 39812323,
        "shipment_stop_id": null,
        "status_location_id": null,
        "actual_created_at": "2024-11-11T02:30:00+00:00",
        "remarks": null,
        "created_at": null,
        "updated_at": null,
        "obc_asset_id": null,
        "driver_id": null,
        "status_code": "LO",
        "status_reason_code": null,
        "is_exception": false,
        "status_type": 1,
        "message_id": null,
        "longitude": -83.587433,
        "latitude": 42.004097,
        "processed_at": "2024-11-11 05:44:17.025576+00:00",
        "trailer_number": null,
        "status_details": "{\"last_reported_at\": \"2024-11-11T01:30:00Z\", \"current_latitude\": 42.004097, \"current_longitude\": -83.587433, \"current_city\": \"Maybee\", \"current_state\": \"MI\", \"current_postal_code\": \"48159\", \"current_country\": \"US\", \"status_code\": \"LO\", \"reported_at\": \"2024-11-11T02:30:00Z\", \"reported_at_local\": \"2024-11-10 21:30:00\", \"created_at\": \"2024-11-11T05:44:16.042202Z\"}",
        "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
        "actor_type": "system",
        "actor_email": "test@freightverify-api.com",
        "rail_asset_id": null,
        "equipment_desc": null
    }
}

Position Event at Detroit Dest:- 8c1b380a-24bc-4194-bd4b-e5fbe40cdea4
Request:-
{
    "carrier": {
        "scac": "TEST",
        "fvCarrierId": "FV0834338A"
    },
    "location": {
        "latitude": 42.216,
        "longitude": -83.355
    },
    "eventDetail": {
        "eventDate": "{{destination_actual_delivery}}",
        "event": "LO"
    }
}
Response:-
{
    "shipment_status": {
        "id": 3255223087,
        "organization_id": 1003,
        "user_id": null,
        "shipment_id": 39812323,
        "shipment_stop_id": null,
        "status_location_id": null,
        "actual_created_at": "2024-11-11T03:30:00+00:00",
        "remarks": null,
        "created_at": null,
        "updated_at": null,
        "obc_asset_id": null,
        "driver_id": null,
        "status_code": "LO",
        "status_reason_code": null,
        "is_exception": false,
        "status_type": 1,
        "message_id": null,
        "longitude": -83.355,
        "latitude": 42.216,
        "processed_at": "2024-11-11 05:46:10.435776+00:00",
        "trailer_number": null,
        "status_details": "{\"last_reported_at\": \"2024-11-11T02:30:00Z\", \"current_latitude\": 42.216, \"current_longitude\": -83.355, \"current_city\": \"Detroit\", \"current_state\": \"MI\", \"current_postal_code\": \"48242\", \"current_country\": \"US\", \"status_code\": \"LO\", \"reported_at\": \"2024-11-11T03:30:00Z\", \"reported_at_local\": \"2024-11-10 22:30:00\", \"created_at\": \"2024-11-11T05:46:08.541823Z\"}",
        "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
        "actor_type": "system",
        "actor_email": "test@freightverify-api.com",
        "rail_asset_id": null,
        "equipment_desc": null
    }
}

Carrier Arrival Event-Detroit:- 8e8855a8-b510-4688-8939-70b66f110912
Request:-
{
    "carrier": {
        "scac": "TEST",
        "fvCarrierId": "FV0834338A"
    },
    "stopSequence": 2,
    "eventDetail": {
        "eventDate": "{{destination_actual_delivery}}",
        "event": "X1",
        "reason": "NS"
    }
}
Response:-
{
    "shipment_status": {
        "id": 3255223090,
        "organization_id": 1003,
        "user_id": null,
        "shipment_id": 39812323,
        "shipment_stop_id": 288481214,
        "status_location_id": null,
        "actual_created_at": "2024-11-11T03:30:00+00:00",
        "remarks": null,
        "created_at": null,
        "updated_at": null,
        "obc_asset_id": null,
        "driver_id": null,
        "status_code": "X1",
        "status_reason_code": "NS",
        "is_exception": false,
        "status_type": 1,
        "message_id": null,
        "longitude": null,
        "latitude": null,
        "processed_at": "2024-11-11 05:47:09.936540+00:00",
        "trailer_number": null,
        "status_details": "{\"last_reported_at\": \"2024-11-11T03:30:00Z\", \"current_latitude\": 42.216, \"current_longitude\": -83.355, \"current_city\": \"Detroit\", \"current_state\": \"MI\", \"current_postal_code\": \"48242\", \"current_country\": \"US\", \"status_code\": \"X1\", \"reported_at\": \"2024-11-11T03:30:00Z\", \"reported_at_local\": \"2024-11-10 22:30:00\", \"created_at\": \"2024-11-11T05:47:09.793521Z\", \"remaining_miles\": 0}",
        "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
        "actor_type": "system",
        "actor_email": "test@freightverify-api.com",
        "rail_asset_id": null,
        "equipment_desc": null
    }
}


Validate Shipment:- 92729caf-96db-4d2c-911a-7de0eb71fe23
Request:-
https://{{gateway_url}}/shipping-ng/shipments?shipment_id={{shipment_id}}&pageNumber=0&pageSize=20&sortColumn=destination_earliest_arrival&reverseSort=0
Response:-
{
    "meta": {
        "totalPages": 131,
        "currentPage": 0,
        "totalCount": 2605
    },
    "data": [
        {
            "id": 39801447,
            "actor_type": "system",
            "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
            "actor_email": "test@freightverify-api.com",
            "fv_id": "FV2690474A",
            "created_by_org_id": 1004,
            "creator_shipment_id": "INZX112GZR1",
            "total_distance": 3487.9233966392894,
            "progress": 100,
            "status_updated_at": null,
            "obc_asset_id": "OCEAN-ASSET",
            "created_at": "2024-09-19T17:50:17.801093",
            "updated_at": "2024-09-19T17:50:25.201102",
            "is_accepted": null,
            "is_completed": null,
            "current_status": "FV_AUP",
            "active_status": "in_transit",
            "active_until": "2024-11-11T17:00:00",
            "eta": "2024-10-12T17:00:00",
            "current_exception": null,
            "remaining_distance": null,
            "message_id": null,
            "is_behind_schedule": false,
            "picked_up_at": null,
            "delivered_at": null,
            "mode_id": 5,
            "leg": false,
            "mode_name": "Ocean",
            "trailer_number": null,
            "carrier_organization_id": 1003,
            "carrier_name": "TEST-Carrier",
            "carrier_fv_id": "FV0834338A",
            "carrier_mc_number": null,
            "carrier_scac": "TEST",
            "origin_code": "LNDN",
            "origin_name": "Port of London",
            "origin_location_id": 271418,
            "origin_location_actual_id": 18481377,
            "origin_address": "4988 Harbor Rd.",
            "origin_city": "Tilbury",
            "origin_state": "LND",
            "origin_postal_code": "SW15 5PU",
            "origin_country": "GB",
            "origin_lad_id": 19,
            "origin_lad_name": "Ocean Port",
            "origin_pickup_window": [
                1726765200.0,
                1726851600.0
            ],
            "origin_earliest_arrival": "2024-09-19T17:00:00",
            "origin_latest_arrival": "2024-09-20T17:00:00",
            "origin_distance": null,
            "origin_remaining_distance": null,
            "origin_calculated_eta": null,
            "origin_actual_arrival": "2024-09-20T05:00:00",
            "origin_actual_departure": "2024-09-21T17:00:00",
            "origin_stop_identifier": null,
            "destination_code": "USNWK",
            "destination_name": "Port Newark USNWK",
            "destination_location_id": 12253301,
            "destination_location_actual_id": 10767920,
            "destination_address": "3276 Industry Way",
            "destination_city": "Newark",
            "destination_state": "NJ ",
            "destination_postal_code": "07099",
            "destination_country": "US",
            "destination_lad_id": 29,
            "destination_lad_name": "Ocean Port",
            "destination_distance": null,
            "destination_remaining_distance": null,
            "destination_calculated_eta": null,
            "destination_actual_arrival": "2024-10-12T05:00:00",
            "destination_frozen_eta": null,
            "destination_frozen_eta_reason": null,
            "destination_actual_departure": null,
            "destination_stop_identifier": null,
            "destination_delivery_window": [
                1728666000.0,
                1728752400.0
            ],
            "destination_earliest_arrival": "2024-10-11T17:00:00",
            "destination_latest_arrival": "2024-10-12T17:00:00",
            "is_rack_return": false,
            "line_of_business_id": 2,
            "tracking_window": [
                1726160400.0,
                1731344400.0
            ],
            "tracking_disabled": null,
            "pro_number": "OCEAN-PRONUM",
            "rail_asset_id": null,
            "route_number": "OCEAN-ROUTE",
            "reference_number": null,
            "last_status_update": "2024-09-19T18:36:27.013392",
            "destination_eta": null,
            "current_city": null,
            "current_state": null,
            "remaining_miles": null,
            "current_country": "Ocean",
            "current_latitude": 40.67241,
            "current_longitude": -74.06925,
            "current_reported_at": "2024-10-12T05:00:00",
            "submode_id": null,
            "parent_shipment_id": null,
            "trip_plan_number": null,
            "current_road_organization_id": null,
            "current_road_name": null,
            "current_road_scac": null,
            "status_type_name": null,
            "status_name": null,
            "rail_train_id": null,
            "rail_loaded_status": null,
            "loaded_status": null,
            "shipment_reference_details": [
                {
                    "value": "",
                    "qualifier": "order_number",
                    "shipment_id": 39801447
                },
                {
                    "value": "OCEAN-PART1 (500)",
                    "qualifier": "part",
                    "shipment_id": 39801447
                },
                {
                    "value": "OCEAN-PART2 (2000)",
                    "qualifier": "part",
                    "shipment_id": 39801447
                },
                {
                    "value": "OCEAN-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39801447
                }
            ],
            "shipment_details": {
                "mode": "Ocean",
                "hasParts": true,
                "relation": null,
                "sub_mode": null,
                "major_mode": "Ocean",
                "is_multileg": false,
                "line_of_business": "inbound",
                "related_shipments": null,
                "stop_count_for_multistop": 2,
                "haul_away_tracking_window": "[\"2024-09-12 17:00:00\",\"2024-11-11 17:00:00\"]",
                "origin_arrived_at_received_ts": "2024-09-23T15:36:28.659951",
                "destination_arrived_at_received_ts": "2024-09-19T18:36:27.397594"
            },
            "origin_region": {
                "region": [
                    "EU"
                ]
            },
            "destination_region": {
                "region": [
                    "NA"
                ]
            },
            "shipment_stop_count": 2,
            "watched": false,
            "comments_count": null,
            "user_has_alert_me_subscription": false,
            "full_count": 2605,
            "current_location": {
                "current_city": null,
                "current_state": null,
                "current_country": "Ocean",
                "distance_progress": "100%",
                "longitude": -74.06925,
                "latitude": 40.67241,
                "remaining_miles": null,
                "reported_at": "2024-10-12T05:00:00",
                "destination_eta": null,
                "updates": [
                    {
                        "time": "2024-10-12T05:00:00",
                        "longitude": -74.06925,
                        "latitude": 40.67241
                    }
                ]
            },
            "active_status_ng": "Active",
            "current_status_ng": "",
            "active_exceptions_ng": "",
            "shipment_type_ng": "Inbound",
            "service_code": null,
            "on_time_percentage": null,
            "has_event_refs": false,
            "origin_location_code": "LNDN",
            "destination_location_code": "USNWK",
            "tracking_window_formatted": [
                "2024-09-12T17:00:00",
                "2024-11-11T17:00:00"
            ],
            "trailer_equipment_number": []
        },
        {
            "id": 39799971,
            "actor_type": null,
            "actor_id": null,
            "actor_email": null,
            "fv_id": null,
            "created_by_org_id": 1004,
            "creator_shipment_id": "JQ0ABEVUGJ",
            "total_distance": 4005.480504404747,
            "progress": null,
            "status_updated_at": null,
            "obc_asset_id": null,
            "created_at": "2024-09-07T20:31:10.199856",
            "updated_at": "2024-09-07T20:31:22.758267",
            "is_accepted": null,
            "is_completed": null,
            "current_status": null,
            "active_status": "asset_pending",
            "active_until": "2024-11-11T20:31:00",
            "eta": null,
            "current_exception": "missed_delivery_exceptions",
            "remaining_distance": null,
            "message_id": null,
            "is_behind_schedule": false,
            "picked_up_at": null,
            "delivered_at": null,
            "mode_id": 6,
            "leg": null,
            "mode_name": "Multimodal",
            "trailer_number": null,
            "carrier_organization_id": 1003,
            "carrier_name": "TEST-Carrier",
            "carrier_fv_id": "FV0834338A",
            "carrier_mc_number": null,
            "carrier_scac": "TEST",
            "origin_code": "PITT",
            "origin_name": "Pittsburgh Supplier",
            "origin_location_id": 288497,
            "origin_location_actual_id": 288533,
            "origin_address": "600 Grant St.",
            "origin_city": "Pittsburgh",
            "origin_state": "PA ",
            "origin_postal_code": "15272",
            "origin_country": "US",
            "origin_lad_id": 32,
            "origin_lad_name": "Dealer",
            "origin_pickup_window": [
                1725741060.0,
                1725827460.0
            ],
            "origin_earliest_arrival": "2024-09-07T20:31:00",
            "origin_latest_arrival": "2024-09-08T20:31:00",
            "origin_distance": null,
            "origin_remaining_distance": null,
            "origin_calculated_eta": null,
            "origin_actual_arrival": null,
            "origin_actual_departure": null,
            "origin_stop_identifier": null,
            "destination_code": "SHEF",
            "destination_name": "Sheffield Plant",
            "destination_location_id": 271419,
            "destination_location_actual_id": 18481402,
            "destination_address": "41794 Main St.",
            "destination_city": "Sheffield",
            "destination_state": "England",
            "destination_postal_code": "S1 1GL",
            "destination_country": "GB",
            "destination_lad_id": 14,
            "destination_lad_name": "Customer Plant",
            "destination_distance": null,
            "destination_remaining_distance": null,
            "destination_calculated_eta": "2024-10-12T20:31:00",
            "destination_actual_arrival": null,
            "destination_frozen_eta": null,
            "destination_frozen_eta_reason": null,
            "destination_actual_departure": null,
            "destination_stop_identifier": null,
            "destination_delivery_window": [
                1728678660.0,
                1728765060.0
            ],
            "destination_earliest_arrival": "2024-10-11T20:31:00",
            "destination_latest_arrival": "2024-10-12T20:31:00",
            "is_rack_return": false,
            "line_of_business_id": 2,
            "tracking_window": [
                1725739266.0,
                1731357060.0
            ],
            "tracking_disabled": null,
            "pro_number": null,
            "rail_asset_id": null,
            "route_number": null,
            "reference_number": null,
            "last_status_update": null,
            "destination_eta": null,
            "current_city": null,
            "current_state": null,
            "remaining_miles": null,
            "current_country": null,
            "current_latitude": null,
            "current_longitude": null,
            "current_reported_at": null,
            "submode_id": null,
            "parent_shipment_id": null,
            "trip_plan_number": null,
            "current_road_organization_id": null,
            "current_road_name": null,
            "current_road_scac": null,
            "status_type_name": null,
            "status_name": null,
            "rail_train_id": null,
            "rail_loaded_status": null,
            "loaded_status": null,
            "shipment_reference_details": [
                {
                    "value": "MULTIMODAL-PART1 (2500)",
                    "qualifier": "part",
                    "shipment_id": 39799973
                },
                {
                    "value": "MULTIMODAL-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39799973
                },
                {
                    "value": "MULTIMODAL-PART1 (2500)",
                    "qualifier": "part",
                    "shipment_id": 39799974
                },
                {
                    "value": "MULTIMODAL-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39799974
                },
                {
                    "value": "MULTIMODAL-PART1 (2500)",
                    "qualifier": "part",
                    "shipment_id": 39799976
                },
                {
                    "value": "MULTIMODAL-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39799976
                },
                {
                    "value": "AAAKDWTSKSXDHC9PF",
                    "qualifier": "XVIN",
                    "shipment_id": 39799976
                }
            ],
            "shipment_details": {
                "mode": "Multimodal",
                "relation": "Parent",
                "sub_mode": null,
                "major_mode": "Multimodal",
                "is_multileg": true,
                "line_of_business": "inbound",
                "related_shipments": [
                    {
                        "active_status": "asset_pending",
                        "trailer_number": null,
                        "child_shipment_id": 39799973,
                        "current_exception": "missed_delivery_exceptions",
                        "creator_shipment_id": "JQ0ABEVUGJ-2",
                        "origin_pickup_window": "[\"2024-09-11 20:31:00\",\"2024-09-12 20:31:00\"]",
                        "destination_delivery_window": "[\"2024-09-28 20:31:00\",\"2024-09-29 20:31:00\"]"
                    },
                    {
                        "active_status": "asset_pending",
                        "trailer_number": null,
                        "child_shipment_id": 39799974,
                        "current_exception": "missed_delivery_exceptions",
                        "creator_shipment_id": "JQ0ABEVUGJ-3",
                        "origin_pickup_window": "[\"2024-10-04 20:31:00\",\"2024-10-05 20:31:00\"]",
                        "destination_delivery_window": "[\"2024-10-11 20:31:00\",\"2024-10-12 20:31:00\"]"
                    },
                    {
                        "active_status": "in_transit",
                        "trailer_number": "TRUCK-TRAILER-FV",
                        "child_shipment_id": 39799976,
                        "current_exception": "missed_delivery_exceptions",
                        "creator_shipment_id": "JQ0ABEVUGJ-1",
                        "origin_pickup_window": "[\"2024-09-07 20:31:00\",\"2024-09-08 20:31:00\"]",
                        "destination_delivery_window": "[\"2024-09-08 20:31:00\",\"2024-09-09 20:31:00\"]"
                    }
                ],
                "haul_away_tracking_window": "[\"2024-09-07 20:01:06\",\"2024-11-11 20:31:00\"]"
            },
            "origin_region": {
                "region": [
                    "NA"
                ]
            },
            "destination_region": {
                "region": [
                    "EU"
                ]
            },
            "shipment_stop_count": 2,
            "watched": false,
            "comments_count": null,
            "user_has_alert_me_subscription": false,
            "full_count": 2605,
            "current_location": {
                "current_city": null,
                "current_state": null,
                "current_country": null,
                "distance_progress": "null",
                "longitude": null,
                "latitude": null,
                "remaining_miles": null,
                "reported_at": null,
                "destination_eta": null,
                "updates": []
            },
            "active_status_ng": "Pending: Asset ID",
            "current_status_ng": "",
            "active_exceptions_ng": "Missed Drop-Off",
            "shipment_type_ng": "Inbound",
            "service_code": null,
            "on_time_percentage": null,
            "has_event_refs": false,
            "origin_location_code": "PITT",
            "destination_location_code": "SHEF",
            "tracking_window_formatted": [
                "2024-09-07T20:01:06",
                "2024-11-11T20:31:00"
            ],
            "trailer_equipment_number": [
                "TRUCK-TRAILER-FV"
            ]
        },
        {
            "id": 39800035,
            "actor_type": null,
            "actor_id": null,
            "actor_email": null,
            "fv_id": null,
            "created_by_org_id": 1004,
            "creator_shipment_id": "RQF8SV82CD",
            "total_distance": 4005.480504404747,
            "progress": null,
            "status_updated_at": null,
            "obc_asset_id": null,
            "created_at": "2024-09-07T20:41:00.647879",
            "updated_at": "2024-09-07T20:41:06.552560",
            "is_accepted": null,
            "is_completed": null,
            "current_status": null,
            "active_status": "asset_pending",
            "active_until": "2024-11-11T20:40:00",
            "eta": null,
            "current_exception": "missed_delivery_exceptions",
            "remaining_distance": null,
            "message_id": null,
            "is_behind_schedule": false,
            "picked_up_at": null,
            "delivered_at": null,
            "mode_id": 6,
            "leg": null,
            "mode_name": "Multimodal",
            "trailer_number": null,
            "carrier_organization_id": 1003,
            "carrier_name": "TEST-Carrier",
            "carrier_fv_id": "FV0834338A",
            "carrier_mc_number": null,
            "carrier_scac": "TEST",
            "origin_code": "PITT",
            "origin_name": "Pittsburgh Supplier",
            "origin_location_id": 288497,
            "origin_location_actual_id": 288533,
            "origin_address": "600 Grant St.",
            "origin_city": "Pittsburgh",
            "origin_state": "PA ",
            "origin_postal_code": "15272",
            "origin_country": "US",
            "origin_lad_id": 32,
            "origin_lad_name": "Dealer",
            "origin_pickup_window": [
                1725741600.0,
                1725828000.0
            ],
            "origin_earliest_arrival": "2024-09-07T20:40:00",
            "origin_latest_arrival": "2024-09-08T20:40:00",
            "origin_distance": null,
            "origin_remaining_distance": null,
            "origin_calculated_eta": null,
            "origin_actual_arrival": null,
            "origin_actual_departure": null,
            "origin_stop_identifier": null,
            "destination_code": "SHEF",
            "destination_name": "Sheffield Plant",
            "destination_location_id": 271419,
            "destination_location_actual_id": 18481402,
            "destination_address": "41794 Main St.",
            "destination_city": "Sheffield",
            "destination_state": "England",
            "destination_postal_code": "S1 1GL",
            "destination_country": "GB",
            "destination_lad_id": 14,
            "destination_lad_name": "Customer Plant",
            "destination_distance": null,
            "destination_remaining_distance": null,
            "destination_calculated_eta": "2024-10-12T20:40:00",
            "destination_actual_arrival": null,
            "destination_frozen_eta": null,
            "destination_frozen_eta_reason": null,
            "destination_actual_departure": null,
            "destination_stop_identifier": null,
            "destination_delivery_window": [
                1728679200.0,
                1728765600.0
            ],
            "destination_earliest_arrival": "2024-10-11T20:40:00",
            "destination_latest_arrival": "2024-10-12T20:40:00",
            "is_rack_return": false,
            "line_of_business_id": 2,
            "tracking_window": [
                1725739857.0,
                1731357600.0
            ],
            "tracking_disabled": null,
            "pro_number": null,
            "rail_asset_id": null,
            "route_number": null,
            "reference_number": null,
            "last_status_update": null,
            "destination_eta": null,
            "current_city": null,
            "current_state": null,
            "remaining_miles": null,
            "current_country": null,
            "current_latitude": null,
            "current_longitude": null,
            "current_reported_at": null,
            "submode_id": null,
            "parent_shipment_id": null,
            "trip_plan_number": null,
            "current_road_organization_id": null,
            "current_road_name": null,
            "current_road_scac": null,
            "status_type_name": null,
            "status_name": null,
            "rail_train_id": null,
            "rail_loaded_status": null,
            "loaded_status": null,
            "shipment_reference_details": [
                {
                    "value": "MULTIMODAL-PART1 (2500)",
                    "qualifier": "part",
                    "shipment_id": 39800039
                },
                {
                    "value": "MULTIMODAL-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39800039
                },
                {
                    "value": "MULTIMODAL-PART1 (2500)",
                    "qualifier": "part",
                    "shipment_id": 39800042
                },
                {
                    "value": "MULTIMODAL-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39800042
                },
                {
                    "value": "MULTIMODAL-PART1 (2500)",
                    "qualifier": "part",
                    "shipment_id": 39800043
                },
                {
                    "value": "MULTIMODAL-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39800043
                }
            ],
            "shipment_details": {
                "mode": "Multimodal",
                "relation": "Parent",
                "sub_mode": null,
                "major_mode": "Multimodal",
                "is_multileg": true,
                "line_of_business": "inbound",
                "related_shipments": [
                    {
                        "active_status": "asset_pending",
                        "trailer_number": null,
                        "child_shipment_id": 39800039,
                        "current_exception": "missed_delivery_exceptions",
                        "creator_shipment_id": "RQF8SV82CD-1",
                        "origin_pickup_window": "[\"2024-09-07 20:40:00\",\"2024-09-08 20:40:00\"]",
                        "destination_delivery_window": "[\"2024-09-08 20:40:00\",\"2024-09-09 20:40:00\"]"
                    },
                    {
                        "active_status": "asset_pending",
                        "trailer_number": null,
                        "child_shipment_id": 39800042,
                        "current_exception": "missed_delivery_exceptions",
                        "creator_shipment_id": "RQF8SV82CD-2",
                        "origin_pickup_window": "[\"2024-09-11 20:40:00\",\"2024-09-12 20:40:00\"]",
                        "destination_delivery_window": "[\"2024-09-28 20:40:00\",\"2024-09-29 20:40:00\"]"
                    },
                    {
                        "active_status": "asset_pending",
                        "trailer_number": null,
                        "child_shipment_id": 39800043,
                        "current_exception": "missed_delivery_exceptions",
                        "creator_shipment_id": "RQF8SV82CD-3",
                        "origin_pickup_window": "[\"2024-10-04 20:40:00\",\"2024-10-05 20:40:00\"]",
                        "destination_delivery_window": "[\"2024-10-11 20:40:00\",\"2024-10-12 20:40:00\"]"
                    }
                ],
                "haul_away_tracking_window": "[\"2024-09-07 20:10:57\",\"2024-11-11 20:40:00\"]"
            },
            "origin_region": {
                "region": [
                    "NA"
                ]
            },
            "destination_region": {
                "region": [
                    "EU"
                ]
            },
            "shipment_stop_count": 2,
            "watched": false,
            "comments_count": null,
            "user_has_alert_me_subscription": false,
            "full_count": 2605,
            "current_location": {
                "current_city": null,
                "current_state": null,
                "current_country": null,
                "distance_progress": "null",
                "longitude": null,
                "latitude": null,
                "remaining_miles": null,
                "reported_at": null,
                "destination_eta": null,
                "updates": []
            },
            "active_status_ng": "Pending: Asset ID",
            "current_status_ng": "",
            "active_exceptions_ng": "Missed Drop-Off",
            "shipment_type_ng": "Inbound",
            "service_code": null,
            "on_time_percentage": null,
            "has_event_refs": false,
            "origin_location_code": "PITT",
            "destination_location_code": "SHEF",
            "tracking_window_formatted": [
                "2024-09-07T20:10:57",
                "2024-11-11T20:40:00"
            ],
            "trailer_equipment_number": []
        },
        {
            "id": 39800034,
            "actor_type": null,
            "actor_id": null,
            "actor_email": null,
            "fv_id": null,
            "created_by_org_id": 1004,
            "creator_shipment_id": "D3ETE7XWI8",
            "total_distance": 4005.480504404747,
            "progress": null,
            "status_updated_at": null,
            "obc_asset_id": null,
            "created_at": "2024-09-07T20:40:59.928215",
            "updated_at": "2024-09-07T20:41:04.123559",
            "is_accepted": null,
            "is_completed": null,
            "current_status": null,
            "active_status": "asset_pending",
            "active_until": "2024-11-11T20:40:00",
            "eta": null,
            "current_exception": "missed_delivery_exceptions",
            "remaining_distance": null,
            "message_id": null,
            "is_behind_schedule": false,
            "picked_up_at": null,
            "delivered_at": null,
            "mode_id": 6,
            "leg": null,
            "mode_name": "Multimodal",
            "trailer_number": null,
            "carrier_organization_id": 1003,
            "carrier_name": "TEST-Carrier",
            "carrier_fv_id": "FV0834338A",
            "carrier_mc_number": null,
            "carrier_scac": "TEST",
            "origin_code": "PITT",
            "origin_name": "Pittsburgh Supplier",
            "origin_location_id": 288497,
            "origin_location_actual_id": 288533,
            "origin_address": "600 Grant St.",
            "origin_city": "Pittsburgh",
            "origin_state": "PA ",
            "origin_postal_code": "15272",
            "origin_country": "US",
            "origin_lad_id": 32,
            "origin_lad_name": "Dealer",
            "origin_pickup_window": [
                1725741600.0,
                1725828000.0
            ],
            "origin_earliest_arrival": "2024-09-07T20:40:00",
            "origin_latest_arrival": "2024-09-08T20:40:00",
            "origin_distance": null,
            "origin_remaining_distance": null,
            "origin_calculated_eta": null,
            "origin_actual_arrival": null,
            "origin_actual_departure": null,
            "origin_stop_identifier": null,
            "destination_code": "SHEF",
            "destination_name": "Sheffield Plant",
            "destination_location_id": 271419,
            "destination_location_actual_id": 18481402,
            "destination_address": "41794 Main St.",
            "destination_city": "Sheffield",
            "destination_state": "England",
            "destination_postal_code": "S1 1GL",
            "destination_country": "GB",
            "destination_lad_id": 14,
            "destination_lad_name": "Customer Plant",
            "destination_distance": null,
            "destination_remaining_distance": null,
            "destination_calculated_eta": "2024-10-12T20:40:00",
            "destination_actual_arrival": null,
            "destination_frozen_eta": null,
            "destination_frozen_eta_reason": null,
            "destination_actual_departure": null,
            "destination_stop_identifier": null,
            "destination_delivery_window": [
                1728679200.0,
                1728765600.0
            ],
            "destination_earliest_arrival": "2024-10-11T20:40:00",
            "destination_latest_arrival": "2024-10-12T20:40:00",
            "is_rack_return": false,
            "line_of_business_id": 2,
            "tracking_window": [
                1725739856.0,
                1731357600.0
            ],
            "tracking_disabled": null,
            "pro_number": null,
            "rail_asset_id": null,
            "route_number": null,
            "reference_number": null,
            "last_status_update": null,
            "destination_eta": null,
            "current_city": null,
            "current_state": null,
            "remaining_miles": null,
            "current_country": null,
            "current_latitude": null,
            "current_longitude": null,
            "current_reported_at": null,
            "submode_id": null,
            "parent_shipment_id": null,
            "trip_plan_number": null,
            "current_road_organization_id": null,
            "current_road_name": null,
            "current_road_scac": null,
            "status_type_name": null,
            "status_name": null,
            "rail_train_id": null,
            "rail_loaded_status": null,
            "loaded_status": null,
            "shipment_reference_details": [
                {
                    "value": "MULTIMODAL-PART1 (2500)",
                    "qualifier": "part",
                    "shipment_id": 39800036
                },
                {
                    "value": "MULTIMODAL-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39800036
                },
                {
                    "value": "MULTIMODAL-PART1 (2500)",
                    "qualifier": "part",
                    "shipment_id": 39800037
                },
                {
                    "value": "MULTIMODAL-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39800037
                },
                {
                    "value": "MULTIMODAL-PART1 (2500)",
                    "qualifier": "part",
                    "shipment_id": 39800038
                },
                {
                    "value": "MULTIMODAL-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39800038
                }
            ],
            "shipment_details": {
                "mode": "Multimodal",
                "relation": "Parent",
                "sub_mode": null,
                "major_mode": "Multimodal",
                "is_multileg": true,
                "line_of_business": "inbound",
                "related_shipments": [
                    {
                        "active_status": "asset_pending",
                        "trailer_number": null,
                        "child_shipment_id": 39800036,
                        "current_exception": "missed_delivery_exceptions",
                        "creator_shipment_id": "D3ETE7XWI8-1",
                        "origin_pickup_window": "[\"2024-09-07 20:40:00\",\"2024-09-08 20:40:00\"]",
                        "destination_delivery_window": "[\"2024-09-08 20:40:00\",\"2024-09-09 20:40:00\"]"
                    },
                    {
                        "active_status": "asset_pending",
                        "trailer_number": null,
                        "child_shipment_id": 39800037,
                        "current_exception": "missed_delivery_exceptions",
                        "creator_shipment_id": "D3ETE7XWI8-2",
                        "origin_pickup_window": "[\"2024-09-11 20:40:00\",\"2024-09-12 20:40:00\"]",
                        "destination_delivery_window": "[\"2024-09-28 20:40:00\",\"2024-09-29 20:40:00\"]"
                    },
                    {
                        "active_status": "asset_pending",
                        "trailer_number": null,
                        "child_shipment_id": 39800038,
                        "current_exception": "missed_delivery_exceptions",
                        "creator_shipment_id": "D3ETE7XWI8-3",
                        "origin_pickup_window": "[\"2024-10-04 20:40:00\",\"2024-10-05 20:40:00\"]",
                        "destination_delivery_window": "[\"2024-10-11 20:40:00\",\"2024-10-12 20:40:00\"]"
                    }
                ],
                "haul_away_tracking_window": "[\"2024-09-07 20:10:56\",\"2024-11-11 20:40:00\"]"
            },
            "origin_region": {
                "region": [
                    "NA"
                ]
            },
            "destination_region": {
                "region": [
                    "EU"
                ]
            },
            "shipment_stop_count": 2,
            "watched": false,
            "comments_count": null,
            "user_has_alert_me_subscription": false,
            "full_count": 2605,
            "current_location": {
                "current_city": null,
                "current_state": null,
                "current_country": null,
                "distance_progress": "null",
                "longitude": null,
                "latitude": null,
                "remaining_miles": null,
                "reported_at": null,
                "destination_eta": null,
                "updates": []
            },
            "active_status_ng": "Pending: Asset ID",
            "current_status_ng": "",
            "active_exceptions_ng": "Missed Drop-Off",
            "shipment_type_ng": "Inbound",
            "service_code": null,
            "on_time_percentage": null,
            "has_event_refs": false,
            "origin_location_code": "PITT",
            "destination_location_code": "SHEF",
            "tracking_window_formatted": [
                "2024-09-07T20:10:56",
                "2024-11-11T20:40:00"
            ],
            "trailer_equipment_number": []
        },
        {
            "id": 39800040,
            "actor_type": null,
            "actor_id": null,
            "actor_email": null,
            "fv_id": null,
            "created_by_org_id": 1004,
            "creator_shipment_id": "TZ2YWBB2WV",
            "total_distance": 4005.480504404747,
            "progress": null,
            "status_updated_at": null,
            "obc_asset_id": null,
            "created_at": "2024-09-07T20:41:02.972047",
            "updated_at": "2024-09-07T20:41:10.945188",
            "is_accepted": null,
            "is_completed": null,
            "current_status": null,
            "active_status": "asset_pending",
            "active_until": "2024-11-11T20:41:00",
            "eta": null,
            "current_exception": "missed_delivery_exceptions",
            "remaining_distance": null,
            "message_id": null,
            "is_behind_schedule": false,
            "picked_up_at": null,
            "delivered_at": null,
            "mode_id": 6,
            "leg": null,
            "mode_name": "Multimodal",
            "trailer_number": null,
            "carrier_organization_id": 1003,
            "carrier_name": "TEST-Carrier",
            "carrier_fv_id": "FV0834338A",
            "carrier_mc_number": null,
            "carrier_scac": "TEST",
            "origin_code": "PITT",
            "origin_name": "Pittsburgh Supplier",
            "origin_location_id": 288497,
            "origin_location_actual_id": 288533,
            "origin_address": "600 Grant St.",
            "origin_city": "Pittsburgh",
            "origin_state": "PA ",
            "origin_postal_code": "15272",
            "origin_country": "US",
            "origin_lad_id": 32,
            "origin_lad_name": "Dealer",
            "origin_pickup_window": [
                1725741660.0,
                1725828060.0
            ],
            "origin_earliest_arrival": "2024-09-07T20:41:00",
            "origin_latest_arrival": "2024-09-08T20:41:00",
            "origin_distance": null,
            "origin_remaining_distance": null,
            "origin_calculated_eta": null,
            "origin_actual_arrival": null,
            "origin_actual_departure": null,
            "origin_stop_identifier": null,
            "destination_code": "SHEF",
            "destination_name": "Sheffield Plant",
            "destination_location_id": 271419,
            "destination_location_actual_id": 18481402,
            "destination_address": "41794 Main St.",
            "destination_city": "Sheffield",
            "destination_state": "England",
            "destination_postal_code": "S1 1GL",
            "destination_country": "GB",
            "destination_lad_id": 14,
            "destination_lad_name": "Customer Plant",
            "destination_distance": null,
            "destination_remaining_distance": null,
            "destination_calculated_eta": "2024-10-12T20:41:00",
            "destination_actual_arrival": null,
            "destination_frozen_eta": null,
            "destination_frozen_eta_reason": null,
            "destination_actual_departure": null,
            "destination_stop_identifier": null,
            "destination_delivery_window": [
                1728679260.0,
                1728765660.0
            ],
            "destination_earliest_arrival": "2024-10-11T20:41:00",
            "destination_latest_arrival": "2024-10-12T20:41:00",
            "is_rack_return": false,
            "line_of_business_id": 2,
            "tracking_window": [
                1725739861.0,
                1731357660.0
            ],
            "tracking_disabled": null,
            "pro_number": null,
            "rail_asset_id": null,
            "route_number": null,
            "reference_number": null,
            "last_status_update": null,
            "destination_eta": null,
            "current_city": null,
            "current_state": null,
            "remaining_miles": null,
            "current_country": null,
            "current_latitude": null,
            "current_longitude": null,
            "current_reported_at": null,
            "submode_id": null,
            "parent_shipment_id": null,
            "trip_plan_number": null,
            "current_road_organization_id": null,
            "current_road_name": null,
            "current_road_scac": null,
            "status_type_name": null,
            "status_name": null,
            "rail_train_id": null,
            "rail_loaded_status": null,
            "loaded_status": null,
            "shipment_reference_details": [
                {
                    "value": "MULTIMODAL-PART1 (2500)",
                    "qualifier": "part",
                    "shipment_id": 39800045
                },
                {
                    "value": "MULTIMODAL-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39800045
                },
                {
                    "value": "MULTIMODAL-PART1 (2500)",
                    "qualifier": "part",
                    "shipment_id": 39800048
                },
                {
                    "value": "MULTIMODAL-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39800048
                },
                {
                    "value": "MULTIMODAL-PART1 (2500)",
                    "qualifier": "part",
                    "shipment_id": 39800050
                },
                {
                    "value": "MULTIMODAL-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39800050
                }
            ],
            "shipment_details": {
                "mode": "Multimodal",
                "relation": "Parent",
                "sub_mode": null,
                "major_mode": "Multimodal",
                "is_multileg": true,
                "line_of_business": "inbound",
                "related_shipments": [
                    {
                        "active_status": "asset_pending",
                        "trailer_number": null,
                        "child_shipment_id": 39800045,
                        "current_exception": "missed_delivery_exceptions",
                        "creator_shipment_id": "TZ2YWBB2WV-1",
                        "origin_pickup_window": "[\"2024-09-07 20:41:00\",\"2024-09-08 20:41:00\"]",
                        "destination_delivery_window": "[\"2024-09-08 20:41:00\",\"2024-09-09 20:41:00\"]"
                    },
                    {
                        "active_status": "asset_pending",
                        "trailer_number": null,
                        "child_shipment_id": 39800048,
                        "current_exception": "missed_delivery_exceptions",
                        "creator_shipment_id": "TZ2YWBB2WV-2",
                        "origin_pickup_window": "[\"2024-09-11 20:41:00\",\"2024-09-12 20:41:00\"]",
                        "destination_delivery_window": "[\"2024-09-28 20:41:00\",\"2024-09-29 20:41:00\"]"
                    },
                    {
                        "active_status": "asset_pending",
                        "trailer_number": null,
                        "child_shipment_id": 39800050,
                        "current_exception": "missed_delivery_exceptions",
                        "creator_shipment_id": "TZ2YWBB2WV-3",
                        "origin_pickup_window": "[\"2024-10-04 20:41:00\",\"2024-10-05 20:41:00\"]",
                        "destination_delivery_window": "[\"2024-10-11 20:41:00\",\"2024-10-12 20:41:00\"]"
                    }
                ],
                "haul_away_tracking_window": "[\"2024-09-07 20:11:01\",\"2024-11-11 20:41:00\"]"
            },
            "origin_region": {
                "region": [
                    "NA"
                ]
            },
            "destination_region": {
                "region": [
                    "EU"
                ]
            },
            "shipment_stop_count": 2,
            "watched": false,
            "comments_count": null,
            "user_has_alert_me_subscription": false,
            "full_count": 2605,
            "current_location": {
                "current_city": null,
                "current_state": null,
                "current_country": null,
                "distance_progress": "null",
                "longitude": null,
                "latitude": null,
                "remaining_miles": null,
                "reported_at": null,
                "destination_eta": null,
                "updates": []
            },
            "active_status_ng": "Pending: Asset ID",
            "current_status_ng": "",
            "active_exceptions_ng": "Missed Drop-Off",
            "shipment_type_ng": "Inbound",
            "service_code": null,
            "on_time_percentage": null,
            "has_event_refs": false,
            "origin_location_code": "PITT",
            "destination_location_code": "SHEF",
            "tracking_window_formatted": [
                "2024-09-07T20:11:01",
                "2024-11-11T20:41:00"
            ],
            "trailer_equipment_number": []
        },
        {
            "id": 39801451,
            "actor_type": "system",
            "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
            "actor_email": "test@freightverify-api.com",
            "fv_id": "FV8886709A",
            "created_by_org_id": 1004,
            "creator_shipment_id": "AKZ2479O1GN",
            "total_distance": 3487.9233966392894,
            "progress": null,
            "status_updated_at": null,
            "obc_asset_id": "OCEAN-ASSET",
            "created_at": "2024-09-20T17:09:40.122791",
            "updated_at": "2024-09-20T17:09:58.876453",
            "is_accepted": null,
            "is_completed": null,
            "current_status": null,
            "active_status": "in_transit",
            "active_until": "2024-11-12T17:00:00",
            "eta": "2024-10-13T17:00:00",
            "current_exception": "missed_delivery_exceptions",
            "remaining_distance": null,
            "message_id": null,
            "is_behind_schedule": false,
            "picked_up_at": null,
            "delivered_at": null,
            "mode_id": 5,
            "leg": false,
            "mode_name": "Ocean",
            "trailer_number": null,
            "carrier_organization_id": 1003,
            "carrier_name": "TEST-Carrier",
            "carrier_fv_id": "FV0834338A",
            "carrier_mc_number": null,
            "carrier_scac": "TEST",
            "origin_code": "LNDN",
            "origin_name": "Port of London",
            "origin_location_id": 271418,
            "origin_location_actual_id": 18481377,
            "origin_address": "4988 Harbor Rd.",
            "origin_city": "Tilbury",
            "origin_state": "LND",
            "origin_postal_code": "SW15 5PU",
            "origin_country": "GB",
            "origin_lad_id": 19,
            "origin_lad_name": "Ocean Port",
            "origin_pickup_window": [
                1726851600.0,
                1726938000.0
            ],
            "origin_earliest_arrival": "2024-09-20T17:00:00",
            "origin_latest_arrival": "2024-09-21T17:00:00",
            "origin_distance": null,
            "origin_remaining_distance": null,
            "origin_calculated_eta": null,
            "origin_actual_arrival": null,
            "origin_actual_departure": null,
            "origin_stop_identifier": null,
            "destination_code": "USNWK",
            "destination_name": "Port Newark USNWK",
            "destination_location_id": 12253301,
            "destination_location_actual_id": 10767920,
            "destination_address": "3276 Industry Way",
            "destination_city": "Newark",
            "destination_state": "NJ ",
            "destination_postal_code": "07099",
            "destination_country": "US",
            "destination_lad_id": 29,
            "destination_lad_name": "Ocean Port",
            "destination_distance": null,
            "destination_remaining_distance": null,
            "destination_calculated_eta": "2024-10-13T17:00:00",
            "destination_actual_arrival": null,
            "destination_frozen_eta": null,
            "destination_frozen_eta_reason": null,
            "destination_actual_departure": null,
            "destination_stop_identifier": null,
            "destination_delivery_window": [
                1728752400.0,
                1728838800.0
            ],
            "destination_earliest_arrival": "2024-10-12T17:00:00",
            "destination_latest_arrival": "2024-10-13T17:00:00",
            "is_rack_return": false,
            "line_of_business_id": 2,
            "tracking_window": [
                1726246800.0,
                1731430800.0
            ],
            "tracking_disabled": null,
            "pro_number": "OCEAN-PRONUM",
            "rail_asset_id": null,
            "route_number": "OCEAN-ROUTE",
            "reference_number": null,
            "last_status_update": null,
            "destination_eta": null,
            "current_city": null,
            "current_state": null,
            "remaining_miles": null,
            "current_country": null,
            "current_latitude": null,
            "current_longitude": null,
            "current_reported_at": null,
            "submode_id": null,
            "parent_shipment_id": null,
            "trip_plan_number": null,
            "current_road_organization_id": null,
            "current_road_name": null,
            "current_road_scac": null,
            "status_type_name": null,
            "status_name": null,
            "rail_train_id": null,
            "rail_loaded_status": null,
            "loaded_status": null,
            "shipment_reference_details": [
                {
                    "value": "BXWNPBDVNR",
                    "qualifier": "order_number",
                    "shipment_id": 39801451
                },
                {
                    "value": "OCEAN-PART1 (500)",
                    "qualifier": "part",
                    "shipment_id": 39801451
                },
                {
                    "value": "OCEAN-PART2 (2000)",
                    "qualifier": "part",
                    "shipment_id": 39801451
                },
                {
                    "value": "OCEAN-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39801451
                }
            ],
            "shipment_details": {
                "mode": "Ocean",
                "hasParts": true,
                "relation": null,
                "sub_mode": null,
                "major_mode": "Ocean",
                "is_multileg": false,
                "line_of_business": "inbound",
                "related_shipments": null,
                "haul_away_tracking_window": "[\"2024-09-13 17:00:00\",\"2024-11-12 17:00:00\"]"
            },
            "origin_region": {
                "region": [
                    "EU"
                ]
            },
            "destination_region": {
                "region": [
                    "NA"
                ]
            },
            "shipment_stop_count": 2,
            "watched": false,
            "comments_count": null,
            "user_has_alert_me_subscription": false,
            "full_count": 2605,
            "current_location": {
                "current_city": null,
                "current_state": null,
                "current_country": null,
                "distance_progress": "null",
                "longitude": null,
                "latitude": null,
                "remaining_miles": null,
                "reported_at": null,
                "destination_eta": null,
                "updates": []
            },
            "active_status_ng": "Active",
            "current_status_ng": "",
            "active_exceptions_ng": "Missed Drop-Off",
            "shipment_type_ng": "Inbound",
            "service_code": null,
            "on_time_percentage": null,
            "has_event_refs": false,
            "origin_location_code": "LNDN",
            "destination_location_code": "USNWK",
            "tracking_window_formatted": [
                "2024-09-13T17:00:00",
                "2024-11-12T17:00:00"
            ],
            "trailer_equipment_number": []
        },
        {
            "id": 39801452,
            "actor_type": "system",
            "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
            "actor_email": "test@freightverify-api.com",
            "fv_id": "FV1927855A",
            "created_by_org_id": 1004,
            "creator_shipment_id": "AM5Q6RLYH0Y",
            "total_distance": 3487.9233966392894,
            "progress": null,
            "status_updated_at": null,
            "obc_asset_id": null,
            "created_at": "2024-09-20T17:09:59.560780",
            "updated_at": "2024-09-20T17:10:01.617290",
            "is_accepted": null,
            "is_completed": null,
            "current_status": null,
            "active_status": "asset_pending",
            "active_until": "2024-11-12T17:00:00",
            "eta": "2024-10-13T17:00:00",
            "current_exception": "missed_delivery_exceptions",
            "remaining_distance": null,
            "message_id": null,
            "is_behind_schedule": false,
            "picked_up_at": null,
            "delivered_at": null,
            "mode_id": 5,
            "leg": false,
            "mode_name": "Ocean",
            "trailer_number": null,
            "carrier_organization_id": 1003,
            "carrier_name": "TEST-Carrier",
            "carrier_fv_id": "FV0834338A",
            "carrier_mc_number": null,
            "carrier_scac": "TEST",
            "origin_code": "LNDN",
            "origin_name": "Port of London",
            "origin_location_id": 271418,
            "origin_location_actual_id": 18481377,
            "origin_address": "4988 Harbor Rd.",
            "origin_city": "Tilbury",
            "origin_state": "LND",
            "origin_postal_code": "SW15 5PU",
            "origin_country": "GB",
            "origin_lad_id": 19,
            "origin_lad_name": "Ocean Port",
            "origin_pickup_window": [
                1726851600.0,
                1726938000.0
            ],
            "origin_earliest_arrival": "2024-09-20T17:00:00",
            "origin_latest_arrival": "2024-09-21T17:00:00",
            "origin_distance": null,
            "origin_remaining_distance": null,
            "origin_calculated_eta": null,
            "origin_actual_arrival": null,
            "origin_actual_departure": null,
            "origin_stop_identifier": null,
            "destination_code": "USNWK",
            "destination_name": "Port Newark USNWK",
            "destination_location_id": 12253301,
            "destination_location_actual_id": 10767920,
            "destination_address": "3276 Industry Way",
            "destination_city": "Newark",
            "destination_state": "NJ ",
            "destination_postal_code": "07099",
            "destination_country": "US",
            "destination_lad_id": 29,
            "destination_lad_name": "Ocean Port",
            "destination_distance": null,
            "destination_remaining_distance": null,
            "destination_calculated_eta": "2024-10-13T17:00:00",
            "destination_actual_arrival": null,
            "destination_frozen_eta": null,
            "destination_frozen_eta_reason": null,
            "destination_actual_departure": null,
            "destination_stop_identifier": null,
            "destination_delivery_window": [
                1728752400.0,
                1728838800.0
            ],
            "destination_earliest_arrival": "2024-10-12T17:00:00",
            "destination_latest_arrival": "2024-10-13T17:00:00",
            "is_rack_return": false,
            "line_of_business_id": 2,
            "tracking_window": [
                1726246800.0,
                1731430800.0
            ],
            "tracking_disabled": null,
            "pro_number": "OCEAN-PRONUM",
            "rail_asset_id": null,
            "route_number": "OCEAN-ROUTE",
            "reference_number": null,
            "last_status_update": null,
            "destination_eta": null,
            "current_city": null,
            "current_state": null,
            "remaining_miles": null,
            "current_country": null,
            "current_latitude": null,
            "current_longitude": null,
            "current_reported_at": null,
            "submode_id": null,
            "parent_shipment_id": null,
            "trip_plan_number": null,
            "current_road_organization_id": null,
            "current_road_name": null,
            "current_road_scac": null,
            "status_type_name": null,
            "status_name": null,
            "rail_train_id": null,
            "rail_loaded_status": null,
            "loaded_status": null,
            "shipment_reference_details": [
                {
                    "value": "BXWNPBDVNR",
                    "qualifier": "order_number",
                    "shipment_id": 39801452
                },
                {
                    "value": "OCEAN-PART1 (500)",
                    "qualifier": "part",
                    "shipment_id": 39801452
                },
                {
                    "value": "OCEAN-PART2 (2000)",
                    "qualifier": "part",
                    "shipment_id": 39801452
                },
                {
                    "value": "OCEAN-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39801452
                }
            ],
            "shipment_details": {
                "mode": "Ocean",
                "hasParts": true,
                "relation": null,
                "sub_mode": null,
                "major_mode": "Ocean",
                "is_multileg": false,
                "line_of_business": "inbound",
                "related_shipments": null,
                "haul_away_tracking_window": "[\"2024-09-13 17:00:00\",\"2024-11-12 17:00:00\"]"
            },
            "origin_region": {
                "region": [
                    "EU"
                ]
            },
            "destination_region": {
                "region": [
                    "NA"
                ]
            },
            "shipment_stop_count": 2,
            "watched": false,
            "comments_count": null,
            "user_has_alert_me_subscription": false,
            "full_count": 2605,
            "current_location": {
                "current_city": null,
                "current_state": null,
                "current_country": null,
                "distance_progress": "null",
                "longitude": null,
                "latitude": null,
                "remaining_miles": null,
                "reported_at": null,
                "destination_eta": null,
                "updates": []
            },
            "active_status_ng": "Pending: Asset ID",
            "current_status_ng": "",
            "active_exceptions_ng": "Missed Drop-Off",
            "shipment_type_ng": "Inbound",
            "service_code": null,
            "on_time_percentage": null,
            "has_event_refs": false,
            "origin_location_code": "LNDN",
            "destination_location_code": "USNWK",
            "tracking_window_formatted": [
                "2024-09-13T17:00:00",
                "2024-11-12T17:00:00"
            ],
            "trailer_equipment_number": []
        },
        {
            "id": 39801173,
            "actor_type": null,
            "actor_id": null,
            "actor_email": null,
            "fv_id": null,
            "created_by_org_id": 1004,
            "creator_shipment_id": "T7VR3IFY3Q",
            "total_distance": 4003.319376066747,
            "progress": null,
            "status_updated_at": null,
            "obc_asset_id": null,
            "created_at": "2024-09-14T20:40:51.839060",
            "updated_at": "2024-09-14T20:41:14.100250",
            "is_accepted": null,
            "is_completed": null,
            "current_status": null,
            "active_status": "asset_pending",
            "active_until": "2024-11-14T20:41:00",
            "eta": null,
            "current_exception": "missed_delivery_exceptions",
            "remaining_distance": null,
            "message_id": null,
            "is_behind_schedule": false,
            "picked_up_at": null,
            "delivered_at": null,
            "mode_id": 6,
            "leg": null,
            "mode_name": "Multimodal",
            "trailer_number": null,
            "carrier_organization_id": 1003,
            "carrier_name": "TEST-Carrier",
            "carrier_fv_id": "FV0834338A",
            "carrier_mc_number": null,
            "carrier_scac": "TEST",
            "origin_code": "PITT",
            "origin_name": "Pittsburgh Supplier",
            "origin_location_id": 288497,
            "origin_location_actual_id": 288533,
            "origin_address": "600 Grant St.",
            "origin_city": "Pittsburgh",
            "origin_state": "PA ",
            "origin_postal_code": "15272",
            "origin_country": "US",
            "origin_lad_id": 32,
            "origin_lad_name": "Dealer",
            "origin_pickup_window": [
                1726044000.0,
                1726065600.0
            ],
            "origin_earliest_arrival": "2024-09-11T08:40:00",
            "origin_latest_arrival": "2024-09-11T14:40:00",
            "origin_distance": null,
            "origin_remaining_distance": null,
            "origin_calculated_eta": null,
            "origin_actual_arrival": null,
            "origin_actual_departure": null,
            "origin_stop_identifier": null,
            "destination_code": "SHEF",
            "destination_name": "Sheffield Plant",
            "destination_location_id": 271419,
            "destination_location_actual_id": 18481402,
            "destination_address": "41794 Main St.",
            "destination_city": "Sheffield",
            "destination_state": "England",
            "destination_postal_code": "S1 1GL",
            "destination_country": "GB",
            "destination_lad_id": 14,
            "destination_lad_name": "Customer Plant",
            "destination_distance": null,
            "destination_remaining_distance": null,
            "destination_calculated_eta": "2024-09-23T20:40:00",
            "destination_actual_arrival": null,
            "destination_frozen_eta": null,
            "destination_frozen_eta_reason": null,
            "destination_actual_departure": null,
            "destination_stop_identifier": null,
            "destination_delivery_window": [
                1728938460.0,
                1729024860.0
            ],
            "destination_earliest_arrival": "2024-10-14T20:41:00",
            "destination_latest_arrival": "2024-10-15T20:41:00",
            "is_rack_return": false,
            "line_of_business_id": 2,
            "tracking_window": [
                1726042248.0,
                1731616860.0
            ],
            "tracking_disabled": null,
            "pro_number": null,
            "rail_asset_id": null,
            "route_number": null,
            "reference_number": null,
            "last_status_update": null,
            "destination_eta": null,
            "current_city": null,
            "current_state": null,
            "remaining_miles": null,
            "current_country": null,
            "current_latitude": null,
            "current_longitude": null,
            "current_reported_at": null,
            "submode_id": null,
            "parent_shipment_id": null,
            "trip_plan_number": null,
            "current_road_organization_id": null,
            "current_road_name": null,
            "current_road_scac": null,
            "status_type_name": null,
            "status_name": null,
            "rail_train_id": null,
            "rail_loaded_status": null,
            "loaded_status": null,
            "shipment_reference_details": [
                {
                    "value": "MULTIMODAL-PART1 (2500)",
                    "qualifier": "part",
                    "shipment_id": 39801176
                },
                {
                    "value": "MULTIMODAL-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39801176
                },
                {
                    "value": "MULTIMODAL-PART1 (2500)",
                    "qualifier": "part",
                    "shipment_id": 39801180
                },
                {
                    "value": "MULTIMODAL-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39801180
                },
                {
                    "value": "MULTIMODAL-PART1 (2500)",
                    "qualifier": "part",
                    "shipment_id": 39801181
                },
                {
                    "value": "MULTIMODAL-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39801181
                }
            ],
            "shipment_details": {
                "mode": "Multimodal",
                "relation": "Parent",
                "sub_mode": null,
                "major_mode": "Multimodal",
                "is_multileg": true,
                "line_of_business": "inbound",
                "related_shipments": [
                    {
                        "active_status": "asset_pending",
                        "trailer_number": null,
                        "child_shipment_id": 39801176,
                        "current_exception": "missed_delivery_exceptions",
                        "creator_shipment_id": "T7VR3IFY3Q-2",
                        "origin_pickup_window": "[\"2024-09-12 20:40:00\",\"2024-09-13 08:40:00\"]",
                        "destination_delivery_window": "[\"2024-09-16 10:40:00\",\"2024-09-17 08:40:00\"]"
                    },
                    {
                        "active_status": "asset_pending",
                        "trailer_number": null,
                        "child_shipment_id": 39801180,
                        "current_exception": "missed_delivery_exceptions",
                        "creator_shipment_id": "T7VR3IFY3Q-1",
                        "origin_pickup_window": "[\"2024-09-11 08:40:00\",\"2024-09-11 14:40:00\"]",
                        "destination_delivery_window": "[\"2024-09-12 02:40:00\",\"2024-09-12 08:40:00\"]"
                    },
                    {
                        "active_status": "asset_pending",
                        "trailer_number": null,
                        "child_shipment_id": 39801181,
                        "current_exception": "missed_delivery_exceptions",
                        "creator_shipment_id": "T7VR3IFY3Q-3",
                        "origin_pickup_window": "[\"2024-09-17 20:40:00\",\"2024-09-18 14:40:00\"]",
                        "destination_delivery_window": "[\"2024-10-14 20:41:00\",\"2024-10-15 20:41:00\"]"
                    }
                ],
                "haul_away_tracking_window": "[\"2024-09-11 08:10:48\",\"2024-11-14 20:41:00\"]"
            },
            "origin_region": {
                "region": [
                    "NA"
                ]
            },
            "destination_region": {
                "region": [
                    "EU"
                ]
            },
            "shipment_stop_count": 2,
            "watched": false,
            "comments_count": null,
            "user_has_alert_me_subscription": false,
            "full_count": 2605,
            "current_location": {
                "current_city": null,
                "current_state": null,
                "current_country": null,
                "distance_progress": "null",
                "longitude": null,
                "latitude": null,
                "remaining_miles": null,
                "reported_at": null,
                "destination_eta": null,
                "updates": []
            },
            "active_status_ng": "Pending: Asset ID",
            "current_status_ng": "",
            "active_exceptions_ng": "Missed Drop-Off",
            "shipment_type_ng": "Inbound",
            "service_code": null,
            "on_time_percentage": null,
            "has_event_refs": false,
            "origin_location_code": "PITT",
            "destination_location_code": "SHEF",
            "tracking_window_formatted": [
                "2024-09-11T08:10:48",
                "2024-11-14T20:41:00"
            ],
            "trailer_equipment_number": []
        },
        {
            "id": 39801660,
            "actor_type": "system",
            "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
            "actor_email": "test@freightverify-api.com",
            "fv_id": "FV6868462A",
            "created_by_org_id": 1004,
            "creator_shipment_id": "A8YXYUU4AUX",
            "total_distance": 3487.9233966392894,
            "progress": null,
            "status_updated_at": null,
            "obc_asset_id": "OCEAN-ASSET",
            "created_at": "2024-09-23T14:57:08.876234",
            "updated_at": "2024-09-23T14:57:08.876234",
            "is_accepted": null,
            "is_completed": null,
            "current_status": null,
            "active_status": "in_transit",
            "active_until": "2024-11-15T14:00:00",
            "eta": "2024-10-16T14:00:00",
            "current_exception": "missed_delivery_exceptions",
            "remaining_distance": null,
            "message_id": null,
            "is_behind_schedule": false,
            "picked_up_at": null,
            "delivered_at": null,
            "mode_id": 5,
            "leg": false,
            "mode_name": "Ocean",
            "trailer_number": null,
            "carrier_organization_id": 1003,
            "carrier_name": "TEST-Carrier",
            "carrier_fv_id": "FV0834338A",
            "carrier_mc_number": null,
            "carrier_scac": "TEST",
            "origin_code": "LNDN",
            "origin_name": "Port of London",
            "origin_location_id": 271418,
            "origin_location_actual_id": 18481377,
            "origin_address": "4988 Harbor Rd.",
            "origin_city": "Tilbury",
            "origin_state": "LND",
            "origin_postal_code": "SW15 5PU",
            "origin_country": "GB",
            "origin_lad_id": 19,
            "origin_lad_name": "Ocean Port",
            "origin_pickup_window": [
                1727100000.0,
                1727186400.0
            ],
            "origin_earliest_arrival": "2024-09-23T14:00:00",
            "origin_latest_arrival": "2024-09-24T14:00:00",
            "origin_distance": null,
            "origin_remaining_distance": null,
            "origin_calculated_eta": null,
            "origin_actual_arrival": null,
            "origin_actual_departure": null,
            "origin_stop_identifier": null,
            "destination_code": "USNWK",
            "destination_name": "Port Newark USNWK",
            "destination_location_id": 12253301,
            "destination_location_actual_id": 10767920,
            "destination_address": "3276 Industry Way",
            "destination_city": "Newark",
            "destination_state": "NJ ",
            "destination_postal_code": "07099",
            "destination_country": "US",
            "destination_lad_id": 29,
            "destination_lad_name": "Ocean Port",
            "destination_distance": null,
            "destination_remaining_distance": null,
            "destination_calculated_eta": "2024-10-16T14:00:00",
            "destination_actual_arrival": null,
            "destination_frozen_eta": null,
            "destination_frozen_eta_reason": null,
            "destination_actual_departure": null,
            "destination_stop_identifier": null,
            "destination_delivery_window": [
                1729000800.0,
                1729087200.0
            ],
            "destination_earliest_arrival": "2024-10-15T14:00:00",
            "destination_latest_arrival": "2024-10-16T14:00:00",
            "is_rack_return": false,
            "line_of_business_id": 2,
            "tracking_window": [
                1726495200.0,
                1731679200.0
            ],
            "tracking_disabled": null,
            "pro_number": "OCEAN-PRONUM",
            "rail_asset_id": null,
            "route_number": "OCEAN-ROUTE",
            "reference_number": null,
            "last_status_update": null,
            "destination_eta": null,
            "current_city": null,
            "current_state": null,
            "remaining_miles": null,
            "current_country": null,
            "current_latitude": null,
            "current_longitude": null,
            "current_reported_at": null,
            "submode_id": null,
            "parent_shipment_id": null,
            "trip_plan_number": null,
            "current_road_organization_id": null,
            "current_road_name": null,
            "current_road_scac": null,
            "status_type_name": null,
            "status_name": null,
            "rail_train_id": null,
            "rail_loaded_status": null,
            "loaded_status": null,
            "shipment_reference_details": [
                {
                    "value": "29P20T5GL3",
                    "qualifier": "order_number",
                    "shipment_id": 39801660
                },
                {
                    "value": "OCEAN-PART1 (500)",
                    "qualifier": "part",
                    "shipment_id": 39801660
                },
                {
                    "value": "OCEAN-PART2 (2000)",
                    "qualifier": "part",
                    "shipment_id": 39801660
                },
                {
                    "value": "OCEAN-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39801660
                }
            ],
            "shipment_details": {
                "mode": "Ocean",
                "hasParts": true,
                "relation": null,
                "sub_mode": null,
                "major_mode": "Ocean",
                "is_multileg": false,
                "line_of_business": "inbound",
                "related_shipments": null,
                "haul_away_tracking_window": "[\"2024-09-16 14:00:00\",\"2024-11-15 14:00:00\"]"
            },
            "origin_region": {
                "region": [
                    "EU"
                ]
            },
            "destination_region": {
                "region": [
                    "NA"
                ]
            },
            "shipment_stop_count": 2,
            "watched": false,
            "comments_count": null,
            "user_has_alert_me_subscription": false,
            "full_count": 2605,
            "current_location": {
                "current_city": null,
                "current_state": null,
                "current_country": null,
                "distance_progress": "null",
                "longitude": null,
                "latitude": null,
                "remaining_miles": null,
                "reported_at": null,
                "destination_eta": null,
                "updates": []
            },
            "active_status_ng": "Active",
            "current_status_ng": "",
            "active_exceptions_ng": "Missed Drop-Off",
            "shipment_type_ng": "Inbound",
            "service_code": null,
            "on_time_percentage": null,
            "has_event_refs": false,
            "origin_location_code": "LNDN",
            "destination_location_code": "USNWK",
            "tracking_window_formatted": [
                "2024-09-16T14:00:00",
                "2024-11-15T14:00:00"
            ],
            "trailer_equipment_number": []
        },
        {
            "id": 39801663,
            "actor_type": "system",
            "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
            "actor_email": "test@freightverify-api.com",
            "fv_id": "FV1615741A",
            "created_by_org_id": 1004,
            "creator_shipment_id": "A6YGNEZW3J3",
            "total_distance": 3487.9233966392894,
            "progress": null,
            "status_updated_at": null,
            "obc_asset_id": "OCEAN-ASSET",
            "created_at": "2024-09-23T15:27:22.868295",
            "updated_at": "2024-09-23T15:27:27.886157",
            "is_accepted": null,
            "is_completed": null,
            "current_status": "FV_AUP",
            "active_status": "in_transit",
            "active_until": "2024-11-15T15:00:00",
            "eta": "2024-10-16T15:00:00",
            "current_exception": "missed_delivery_exceptions",
            "remaining_distance": null,
            "message_id": null,
            "is_behind_schedule": false,
            "picked_up_at": null,
            "delivered_at": null,
            "mode_id": 5,
            "leg": false,
            "mode_name": "Ocean",
            "trailer_number": null,
            "carrier_organization_id": 1003,
            "carrier_name": "TEST-Carrier",
            "carrier_fv_id": "FV0834338A",
            "carrier_mc_number": null,
            "carrier_scac": "TEST",
            "origin_code": "LNDN",
            "origin_name": "Port of London",
            "origin_location_id": 271418,
            "origin_location_actual_id": 18481377,
            "origin_address": "4988 Harbor Rd.",
            "origin_city": "Tilbury",
            "origin_state": "LND",
            "origin_postal_code": "SW15 5PU",
            "origin_country": "GB",
            "origin_lad_id": 19,
            "origin_lad_name": "Ocean Port",
            "origin_pickup_window": [
                1727103600.0,
                1727190000.0
            ],
            "origin_earliest_arrival": "2024-09-23T15:00:00",
            "origin_latest_arrival": "2024-09-24T15:00:00",
            "origin_distance": null,
            "origin_remaining_distance": null,
            "origin_calculated_eta": null,
            "origin_actual_arrival": "2024-09-24T03:00:00",
            "origin_actual_departure": null,
            "origin_stop_identifier": null,
            "destination_code": "USNWK",
            "destination_name": "Port Newark USNWK",
            "destination_location_id": 12253301,
            "destination_location_actual_id": 10767920,
            "destination_address": "3276 Industry Way",
            "destination_city": "Newark",
            "destination_state": "NJ ",
            "destination_postal_code": "07099",
            "destination_country": "US",
            "destination_lad_id": 29,
            "destination_lad_name": "Ocean Port",
            "destination_distance": null,
            "destination_remaining_distance": null,
            "destination_calculated_eta": "2024-10-16T15:00:00",
            "destination_actual_arrival": null,
            "destination_frozen_eta": null,
            "destination_frozen_eta_reason": null,
            "destination_actual_departure": null,
            "destination_stop_identifier": null,
            "destination_delivery_window": [
                1729004400.0,
                1729090800.0
            ],
            "destination_earliest_arrival": "2024-10-15T15:00:00",
            "destination_latest_arrival": "2024-10-16T15:00:00",
            "is_rack_return": false,
            "line_of_business_id": 2,
            "tracking_window": [
                1726498800.0,
                1731682800.0
            ],
            "tracking_disabled": null,
            "pro_number": "OCEAN-PRONUM",
            "rail_asset_id": null,
            "route_number": "OCEAN-ROUTE",
            "reference_number": null,
            "last_status_update": "2024-09-23T15:28:43.328908",
            "destination_eta": null,
            "current_city": null,
            "current_state": null,
            "remaining_miles": null,
            "current_country": "Ocean",
            "current_latitude": 51.4534,
            "current_longitude": 0.3387,
            "current_reported_at": "2024-10-16T15:00:00",
            "submode_id": null,
            "parent_shipment_id": null,
            "trip_plan_number": null,
            "current_road_organization_id": null,
            "current_road_name": null,
            "current_road_scac": null,
            "status_type_name": null,
            "status_name": null,
            "rail_train_id": null,
            "rail_loaded_status": null,
            "loaded_status": null,
            "shipment_reference_details": [
                {
                    "value": "29P20T5GL3",
                    "qualifier": "order_number",
                    "shipment_id": 39801663
                },
                {
                    "value": "OCEAN-PART1 (500)",
                    "qualifier": "part",
                    "shipment_id": 39801663
                },
                {
                    "value": "OCEAN-PART2 (2000)",
                    "qualifier": "part",
                    "shipment_id": 39801663
                },
                {
                    "value": "OCEAN-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39801663
                }
            ],
            "shipment_details": {
                "mode": "Ocean",
                "hasParts": true,
                "relation": null,
                "sub_mode": null,
                "major_mode": "Ocean",
                "is_multileg": false,
                "line_of_business": "inbound",
                "related_shipments": null,
                "stop_count_for_multistop": 2,
                "haul_away_tracking_window": "[\"2024-09-16 15:00:00\",\"2024-11-15 15:00:00\"]",
                "origin_arrived_at_received_ts": "2024-09-23T15:27:27.427198"
            },
            "origin_region": {
                "region": [
                    "EU"
                ]
            },
            "destination_region": {
                "region": [
                    "NA"
                ]
            },
            "shipment_stop_count": 2,
            "watched": false,
            "comments_count": null,
            "user_has_alert_me_subscription": false,
            "full_count": 2605,
            "current_location": {
                "current_city": null,
                "current_state": null,
                "current_country": "Ocean",
                "distance_progress": "null",
                "longitude": 0.3387,
                "latitude": 51.4534,
                "remaining_miles": null,
                "reported_at": "2024-10-16T15:00:00",
                "destination_eta": null,
                "updates": [
                    {
                        "time": "2024-10-16T15:00:00",
                        "longitude": 0.3387,
                        "latitude": 51.4534
                    }
                ]
            },
            "active_status_ng": "Active",
            "current_status_ng": "",
            "active_exceptions_ng": "Missed Drop-Off",
            "shipment_type_ng": "Inbound",
            "service_code": null,
            "on_time_percentage": null,
            "has_event_refs": false,
            "origin_location_code": "LNDN",
            "destination_location_code": "USNWK",
            "tracking_window_formatted": [
                "2024-09-16T15:00:00",
                "2024-11-15T15:00:00"
            ],
            "trailer_equipment_number": []
        },
        {
            "id": 39801666,
            "actor_type": "system",
            "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
            "actor_email": "test@freightverify-api.com",
            "fv_id": "FV5272200A",
            "created_by_org_id": 1004,
            "creator_shipment_id": "AY44KKBO0VK",
            "total_distance": 3487.9233966392894,
            "progress": null,
            "status_updated_at": null,
            "obc_asset_id": "OCEAN-ASSET",
            "created_at": "2024-09-23T15:58:30.880186",
            "updated_at": "2024-09-23T15:58:38.647248",
            "is_accepted": null,
            "is_completed": null,
            "current_status": "FV_AUP",
            "active_status": "in_transit",
            "active_until": "2024-11-15T15:00:00",
            "eta": "2024-10-16T15:00:00",
            "current_exception": "missed_delivery_exceptions",
            "remaining_distance": null,
            "message_id": null,
            "is_behind_schedule": false,
            "picked_up_at": null,
            "delivered_at": null,
            "mode_id": 5,
            "leg": false,
            "mode_name": "Ocean",
            "trailer_number": null,
            "carrier_organization_id": 1003,
            "carrier_name": "TEST-Carrier",
            "carrier_fv_id": "FV0834338A",
            "carrier_mc_number": null,
            "carrier_scac": "TEST",
            "origin_code": "LNDN",
            "origin_name": "Port of London",
            "origin_location_id": 271418,
            "origin_location_actual_id": 18481377,
            "origin_address": "4988 Harbor Rd.",
            "origin_city": "Tilbury",
            "origin_state": "LND",
            "origin_postal_code": "SW15 5PU",
            "origin_country": "GB",
            "origin_lad_id": 19,
            "origin_lad_name": "Ocean Port",
            "origin_pickup_window": [
                1727103600.0,
                1727190000.0
            ],
            "origin_earliest_arrival": "2024-09-23T15:00:00",
            "origin_latest_arrival": "2024-09-24T15:00:00",
            "origin_distance": null,
            "origin_remaining_distance": null,
            "origin_calculated_eta": null,
            "origin_actual_arrival": "2024-09-24T03:00:00",
            "origin_actual_departure": null,
            "origin_stop_identifier": null,
            "destination_code": "USNWK",
            "destination_name": "Port Newark USNWK",
            "destination_location_id": 12253301,
            "destination_location_actual_id": 10767920,
            "destination_address": "3276 Industry Way",
            "destination_city": "Newark",
            "destination_state": "NJ ",
            "destination_postal_code": "07099",
            "destination_country": "US",
            "destination_lad_id": 29,
            "destination_lad_name": "Ocean Port",
            "destination_distance": null,
            "destination_remaining_distance": null,
            "destination_calculated_eta": "2024-10-16T15:00:00",
            "destination_actual_arrival": null,
            "destination_frozen_eta": null,
            "destination_frozen_eta_reason": null,
            "destination_actual_departure": null,
            "destination_stop_identifier": null,
            "destination_delivery_window": [
                1729004400.0,
                1729090800.0
            ],
            "destination_earliest_arrival": "2024-10-15T15:00:00",
            "destination_latest_arrival": "2024-10-16T15:00:00",
            "is_rack_return": false,
            "line_of_business_id": 2,
            "tracking_window": [
                1726498800.0,
                1731682800.0
            ],
            "tracking_disabled": null,
            "pro_number": "OCEAN-PRONUM",
            "rail_asset_id": null,
            "route_number": "OCEAN-ROUTE",
            "reference_number": null,
            "last_status_update": "2024-09-23T15:58:38.209624",
            "destination_eta": null,
            "current_city": null,
            "current_state": null,
            "remaining_miles": null,
            "current_country": "Ocean",
            "current_latitude": 51.4534,
            "current_longitude": 0.3387,
            "current_reported_at": "2024-09-24T03:00:00",
            "submode_id": null,
            "parent_shipment_id": null,
            "trip_plan_number": null,
            "current_road_organization_id": null,
            "current_road_name": null,
            "current_road_scac": null,
            "status_type_name": null,
            "status_name": null,
            "rail_train_id": null,
            "rail_loaded_status": null,
            "loaded_status": null,
            "shipment_reference_details": [
                {
                    "value": "BXWNPBDVNR",
                    "qualifier": "order_number",
                    "shipment_id": 39801666
                },
                {
                    "value": "OCEAN-PART1 (500)",
                    "qualifier": "part",
                    "shipment_id": 39801666
                },
                {
                    "value": "OCEAN-PART2 (2000)",
                    "qualifier": "part",
                    "shipment_id": 39801666
                },
                {
                    "value": "OCEAN-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39801666
                }
            ],
            "shipment_details": {
                "mode": "Ocean",
                "hasParts": true,
                "relation": null,
                "sub_mode": null,
                "major_mode": "Ocean",
                "is_multileg": false,
                "line_of_business": "inbound",
                "related_shipments": null,
                "stop_count_for_multistop": 2,
                "haul_away_tracking_window": "[\"2024-09-16 15:00:00\",\"2024-11-15 15:00:00\"]",
                "origin_arrived_at_received_ts": "2024-09-23T15:58:35.945714"
            },
            "origin_region": {
                "region": [
                    "EU"
                ]
            },
            "destination_region": {
                "region": [
                    "NA"
                ]
            },
            "shipment_stop_count": 2,
            "watched": false,
            "comments_count": null,
            "user_has_alert_me_subscription": false,
            "full_count": 2605,
            "current_location": {
                "current_city": null,
                "current_state": null,
                "current_country": "Ocean",
                "distance_progress": "null",
                "longitude": 0.3387,
                "latitude": 51.4534,
                "remaining_miles": null,
                "reported_at": "2024-09-24T03:00:00",
                "destination_eta": null,
                "updates": [
                    {
                        "time": "2024-09-24T03:00:00",
                        "longitude": 0.3387,
                        "latitude": 51.4534
                    }
                ]
            },
            "active_status_ng": "Active",
            "current_status_ng": "",
            "active_exceptions_ng": "Missed Drop-Off",
            "shipment_type_ng": "Inbound",
            "service_code": null,
            "on_time_percentage": null,
            "has_event_refs": false,
            "origin_location_code": "LNDN",
            "destination_location_code": "USNWK",
            "tracking_window_formatted": [
                "2024-09-16T15:00:00",
                "2024-11-15T15:00:00"
            ],
            "trailer_equipment_number": []
        },
        {
            "id": 39801662,
            "actor_type": "system",
            "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
            "actor_email": "test@freightverify-api.com",
            "fv_id": "FV0862760A",
            "created_by_org_id": 1004,
            "creator_shipment_id": "ARKC772I9C7",
            "total_distance": 3487.9233966392894,
            "progress": null,
            "status_updated_at": null,
            "obc_asset_id": "OCEAN-ASSET",
            "created_at": "2024-09-23T15:25:31.827831",
            "updated_at": "2024-09-23T15:25:59.588679",
            "is_accepted": null,
            "is_completed": null,
            "current_status": "FV_AUP",
            "active_status": "in_transit",
            "active_until": "2024-11-15T15:00:00",
            "eta": "2024-10-16T15:00:00",
            "current_exception": "missed_delivery_exceptions",
            "remaining_distance": null,
            "message_id": null,
            "is_behind_schedule": false,
            "picked_up_at": null,
            "delivered_at": null,
            "mode_id": 5,
            "leg": false,
            "mode_name": "Ocean",
            "trailer_number": null,
            "carrier_organization_id": 1003,
            "carrier_name": "TEST-Carrier",
            "carrier_fv_id": "FV0834338A",
            "carrier_mc_number": null,
            "carrier_scac": "TEST",
            "origin_code": "LNDN",
            "origin_name": "Port of London",
            "origin_location_id": 271418,
            "origin_location_actual_id": 18481377,
            "origin_address": "4988 Harbor Rd.",
            "origin_city": "Tilbury",
            "origin_state": "LND",
            "origin_postal_code": "SW15 5PU",
            "origin_country": "GB",
            "origin_lad_id": 19,
            "origin_lad_name": "Ocean Port",
            "origin_pickup_window": [
                1727103600.0,
                1727190000.0
            ],
            "origin_earliest_arrival": "2024-09-23T15:00:00",
            "origin_latest_arrival": "2024-09-24T15:00:00",
            "origin_distance": null,
            "origin_remaining_distance": null,
            "origin_calculated_eta": null,
            "origin_actual_arrival": "2024-09-24T03:00:00",
            "origin_actual_departure": null,
            "origin_stop_identifier": null,
            "destination_code": "USNWK",
            "destination_name": "Port Newark USNWK",
            "destination_location_id": 12253301,
            "destination_location_actual_id": 10767920,
            "destination_address": "3276 Industry Way",
            "destination_city": "Newark",
            "destination_state": "NJ ",
            "destination_postal_code": "07099",
            "destination_country": "US",
            "destination_lad_id": 29,
            "destination_lad_name": "Ocean Port",
            "destination_distance": null,
            "destination_remaining_distance": null,
            "destination_calculated_eta": "2024-10-16T15:00:00",
            "destination_actual_arrival": null,
            "destination_frozen_eta": null,
            "destination_frozen_eta_reason": null,
            "destination_actual_departure": null,
            "destination_stop_identifier": null,
            "destination_delivery_window": [
                1729004400.0,
                1729090800.0
            ],
            "destination_earliest_arrival": "2024-10-15T15:00:00",
            "destination_latest_arrival": "2024-10-16T15:00:00",
            "is_rack_return": false,
            "line_of_business_id": 2,
            "tracking_window": [
                1726498800.0,
                1731682800.0
            ],
            "tracking_disabled": null,
            "pro_number": "OCEAN-PRONUM",
            "rail_asset_id": null,
            "route_number": "OCEAN-ROUTE",
            "reference_number": null,
            "last_status_update": "2024-09-23T15:25:59.573972",
            "destination_eta": null,
            "current_city": null,
            "current_state": null,
            "remaining_miles": null,
            "current_country": "Ocean",
            "current_latitude": 51.4534,
            "current_longitude": 0.3387,
            "current_reported_at": "2024-09-24T03:00:00",
            "submode_id": null,
            "parent_shipment_id": null,
            "trip_plan_number": null,
            "current_road_organization_id": null,
            "current_road_name": null,
            "current_road_scac": null,
            "status_type_name": null,
            "status_name": null,
            "rail_train_id": null,
            "rail_loaded_status": null,
            "loaded_status": null,
            "shipment_reference_details": [
                {
                    "value": "29P20T5GL3",
                    "qualifier": "order_number",
                    "shipment_id": 39801662
                },
                {
                    "value": "OCEAN-PART1 (500)",
                    "qualifier": "part",
                    "shipment_id": 39801662
                },
                {
                    "value": "OCEAN-PART2 (2000)",
                    "qualifier": "part",
                    "shipment_id": 39801662
                },
                {
                    "value": "OCEAN-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39801662
                }
            ],
            "shipment_details": {
                "mode": "Ocean",
                "hasParts": true,
                "relation": null,
                "sub_mode": null,
                "major_mode": "Ocean",
                "is_multileg": false,
                "line_of_business": "inbound",
                "related_shipments": null,
                "stop_count_for_multistop": 2,
                "haul_away_tracking_window": "[\"2024-09-16 15:00:00\",\"2024-11-15 15:00:00\"]",
                "origin_arrived_at_received_ts": "2024-09-23T15:26:07.026965"
            },
            "origin_region": {
                "region": [
                    "EU"
                ]
            },
            "destination_region": {
                "region": [
                    "NA"
                ]
            },
            "shipment_stop_count": 2,
            "watched": false,
            "comments_count": null,
            "user_has_alert_me_subscription": false,
            "full_count": 2605,
            "current_location": {
                "current_city": null,
                "current_state": null,
                "current_country": "Ocean",
                "distance_progress": "null",
                "longitude": 0.3387,
                "latitude": 51.4534,
                "remaining_miles": null,
                "reported_at": "2024-09-24T03:00:00",
                "destination_eta": null,
                "updates": [
                    {
                        "time": "2024-09-24T03:00:00",
                        "longitude": 0.3387,
                        "latitude": 51.4534
                    }
                ]
            },
            "active_status_ng": "Active",
            "current_status_ng": "",
            "active_exceptions_ng": "Missed Drop-Off",
            "shipment_type_ng": "Inbound",
            "service_code": null,
            "on_time_percentage": null,
            "has_event_refs": false,
            "origin_location_code": "LNDN",
            "destination_location_code": "USNWK",
            "tracking_window_formatted": [
                "2024-09-16T15:00:00",
                "2024-11-15T15:00:00"
            ],
            "trailer_equipment_number": []
        },
        {
            "id": 39801665,
            "actor_type": "system",
            "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
            "actor_email": "test@freightverify-api.com",
            "fv_id": "FV4899576A",
            "created_by_org_id": 1004,
            "creator_shipment_id": "AYDZ81CVHLV",
            "total_distance": 3487.9233966392894,
            "progress": null,
            "status_updated_at": null,
            "obc_asset_id": "OCEAN-ASSET",
            "created_at": "2024-09-23T15:56:56.657914",
            "updated_at": "2024-09-23T15:57:03.998407",
            "is_accepted": null,
            "is_completed": null,
            "current_status": "FV_AUP",
            "active_status": "in_transit",
            "active_until": "2024-11-15T15:00:00",
            "eta": "2024-10-16T15:00:00",
            "current_exception": "missed_delivery_exceptions",
            "remaining_distance": null,
            "message_id": null,
            "is_behind_schedule": false,
            "picked_up_at": null,
            "delivered_at": null,
            "mode_id": 5,
            "leg": false,
            "mode_name": "Ocean",
            "trailer_number": null,
            "carrier_organization_id": 1003,
            "carrier_name": "TEST-Carrier",
            "carrier_fv_id": "FV0834338A",
            "carrier_mc_number": null,
            "carrier_scac": "TEST",
            "origin_code": "LNDN",
            "origin_name": "Port of London",
            "origin_location_id": 271418,
            "origin_location_actual_id": 18481377,
            "origin_address": "4988 Harbor Rd.",
            "origin_city": "Tilbury",
            "origin_state": "LND",
            "origin_postal_code": "SW15 5PU",
            "origin_country": "GB",
            "origin_lad_id": 19,
            "origin_lad_name": "Ocean Port",
            "origin_pickup_window": [
                1727103600.0,
                1727190000.0
            ],
            "origin_earliest_arrival": "2024-09-23T15:00:00",
            "origin_latest_arrival": "2024-09-24T15:00:00",
            "origin_distance": null,
            "origin_remaining_distance": null,
            "origin_calculated_eta": null,
            "origin_actual_arrival": "2024-09-24T03:00:00",
            "origin_actual_departure": null,
            "origin_stop_identifier": null,
            "destination_code": "USNWK",
            "destination_name": "Port Newark USNWK",
            "destination_location_id": 12253301,
            "destination_location_actual_id": 10767920,
            "destination_address": "3276 Industry Way",
            "destination_city": "Newark",
            "destination_state": "NJ ",
            "destination_postal_code": "07099",
            "destination_country": "US",
            "destination_lad_id": 29,
            "destination_lad_name": "Ocean Port",
            "destination_distance": null,
            "destination_remaining_distance": null,
            "destination_calculated_eta": "2024-10-16T15:00:00",
            "destination_actual_arrival": null,
            "destination_frozen_eta": null,
            "destination_frozen_eta_reason": null,
            "destination_actual_departure": null,
            "destination_stop_identifier": null,
            "destination_delivery_window": [
                1729004400.0,
                1729090800.0
            ],
            "destination_earliest_arrival": "2024-10-15T15:00:00",
            "destination_latest_arrival": "2024-10-16T15:00:00",
            "is_rack_return": false,
            "line_of_business_id": 2,
            "tracking_window": [
                1726498800.0,
                1731682800.0
            ],
            "tracking_disabled": null,
            "pro_number": "OCEAN-PRONUM",
            "rail_asset_id": null,
            "route_number": "OCEAN-ROUTE",
            "reference_number": null,
            "last_status_update": "2024-09-23T15:57:03.555699",
            "destination_eta": null,
            "current_city": null,
            "current_state": null,
            "remaining_miles": null,
            "current_country": "Ocean",
            "current_latitude": 51.4534,
            "current_longitude": 0.3387,
            "current_reported_at": "2024-09-24T03:00:00",
            "submode_id": null,
            "parent_shipment_id": null,
            "trip_plan_number": null,
            "current_road_organization_id": null,
            "current_road_name": null,
            "current_road_scac": null,
            "status_type_name": null,
            "status_name": null,
            "rail_train_id": null,
            "rail_loaded_status": null,
            "loaded_status": null,
            "shipment_reference_details": [
                {
                    "value": "BXWNPBDVNR",
                    "qualifier": "order_number",
                    "shipment_id": 39801665
                },
                {
                    "value": "OCEAN-PART1 (500)",
                    "qualifier": "part",
                    "shipment_id": 39801665
                },
                {
                    "value": "OCEAN-PART2 (2000)",
                    "qualifier": "part",
                    "shipment_id": 39801665
                },
                {
                    "value": "OCEAN-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39801665
                }
            ],
            "shipment_details": {
                "mode": "Ocean",
                "hasParts": true,
                "relation": null,
                "sub_mode": null,
                "major_mode": "Ocean",
                "is_multileg": false,
                "line_of_business": "inbound",
                "related_shipments": null,
                "stop_count_for_multistop": 2,
                "haul_away_tracking_window": "[\"2024-09-16 15:00:00\",\"2024-11-15 15:00:00\"]",
                "origin_arrived_at_received_ts": "2024-09-23T15:57:01.241216"
            },
            "origin_region": {
                "region": [
                    "EU"
                ]
            },
            "destination_region": {
                "region": [
                    "NA"
                ]
            },
            "shipment_stop_count": 2,
            "watched": false,
            "comments_count": null,
            "user_has_alert_me_subscription": false,
            "full_count": 2605,
            "current_location": {
                "current_city": null,
                "current_state": null,
                "current_country": "Ocean",
                "distance_progress": "null",
                "longitude": 0.3387,
                "latitude": 51.4534,
                "remaining_miles": null,
                "reported_at": "2024-09-24T03:00:00",
                "destination_eta": null,
                "updates": [
                    {
                        "time": "2024-09-24T03:00:00",
                        "longitude": 0.3387,
                        "latitude": 51.4534
                    }
                ]
            },
            "active_status_ng": "Active",
            "current_status_ng": "",
            "active_exceptions_ng": "Missed Drop-Off",
            "shipment_type_ng": "Inbound",
            "service_code": null,
            "on_time_percentage": null,
            "has_event_refs": false,
            "origin_location_code": "LNDN",
            "destination_location_code": "USNWK",
            "tracking_window_formatted": [
                "2024-09-16T15:00:00",
                "2024-11-15T15:00:00"
            ],
            "trailer_equipment_number": []
        },
        {
            "id": 39801664,
            "actor_type": "system",
            "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
            "actor_email": "test@freightverify-api.com",
            "fv_id": "FV3877970A",
            "created_by_org_id": 1004,
            "creator_shipment_id": "A75SXLNP5MH",
            "total_distance": 3487.9233966392894,
            "progress": null,
            "status_updated_at": null,
            "obc_asset_id": "OCEAN-ASSET",
            "created_at": "2024-09-23T15:55:42.268149",
            "updated_at": "2024-09-23T15:55:49.871792",
            "is_accepted": null,
            "is_completed": null,
            "current_status": "FV_AUP",
            "active_status": "in_transit",
            "active_until": "2024-11-15T15:00:00",
            "eta": "2024-10-16T15:00:00",
            "current_exception": "missed_delivery_exceptions",
            "remaining_distance": null,
            "message_id": null,
            "is_behind_schedule": false,
            "picked_up_at": null,
            "delivered_at": null,
            "mode_id": 5,
            "leg": false,
            "mode_name": "Ocean",
            "trailer_number": null,
            "carrier_organization_id": 1003,
            "carrier_name": "TEST-Carrier",
            "carrier_fv_id": "FV0834338A",
            "carrier_mc_number": null,
            "carrier_scac": "TEST",
            "origin_code": "LNDN",
            "origin_name": "Port of London",
            "origin_location_id": 271418,
            "origin_location_actual_id": 18481377,
            "origin_address": "4988 Harbor Rd.",
            "origin_city": "Tilbury",
            "origin_state": "LND",
            "origin_postal_code": "SW15 5PU",
            "origin_country": "GB",
            "origin_lad_id": 19,
            "origin_lad_name": "Ocean Port",
            "origin_pickup_window": [
                1727103600.0,
                1727190000.0
            ],
            "origin_earliest_arrival": "2024-09-23T15:00:00",
            "origin_latest_arrival": "2024-09-24T15:00:00",
            "origin_distance": null,
            "origin_remaining_distance": null,
            "origin_calculated_eta": null,
            "origin_actual_arrival": "2024-09-24T03:00:00",
            "origin_actual_departure": null,
            "origin_stop_identifier": null,
            "destination_code": "USNWK",
            "destination_name": "Port Newark USNWK",
            "destination_location_id": 12253301,
            "destination_location_actual_id": 10767920,
            "destination_address": "3276 Industry Way",
            "destination_city": "Newark",
            "destination_state": "NJ ",
            "destination_postal_code": "07099",
            "destination_country": "US",
            "destination_lad_id": 29,
            "destination_lad_name": "Ocean Port",
            "destination_distance": null,
            "destination_remaining_distance": null,
            "destination_calculated_eta": "2024-10-16T15:00:00",
            "destination_actual_arrival": null,
            "destination_frozen_eta": null,
            "destination_frozen_eta_reason": null,
            "destination_actual_departure": null,
            "destination_stop_identifier": null,
            "destination_delivery_window": [
                1729004400.0,
                1729090800.0
            ],
            "destination_earliest_arrival": "2024-10-15T15:00:00",
            "destination_latest_arrival": "2024-10-16T15:00:00",
            "is_rack_return": false,
            "line_of_business_id": 2,
            "tracking_window": [
                1726498800.0,
                1731682800.0
            ],
            "tracking_disabled": null,
            "pro_number": "OCEAN-PRONUM",
            "rail_asset_id": null,
            "route_number": "OCEAN-ROUTE",
            "reference_number": null,
            "last_status_update": "2024-09-23T15:56:14.638540",
            "destination_eta": null,
            "current_city": null,
            "current_state": null,
            "remaining_miles": null,
            "current_country": "Ocean",
            "current_latitude": 51.4534,
            "current_longitude": 0.3387,
            "current_reported_at": "2024-09-24T03:00:00",
            "submode_id": null,
            "parent_shipment_id": null,
            "trip_plan_number": null,
            "current_road_organization_id": null,
            "current_road_name": null,
            "current_road_scac": null,
            "status_type_name": null,
            "status_name": null,
            "rail_train_id": null,
            "rail_loaded_status": null,
            "loaded_status": null,
            "shipment_reference_details": [
                {
                    "value": "BXWNPBDVNR",
                    "qualifier": "order_number",
                    "shipment_id": 39801664
                },
                {
                    "value": "OCEAN-PART1 (500)",
                    "qualifier": "part",
                    "shipment_id": 39801664
                },
                {
                    "value": "OCEAN-PART2 (2000)",
                    "qualifier": "part",
                    "shipment_id": 39801664
                },
                {
                    "value": "OCEAN-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39801664
                }
            ],
            "shipment_details": {
                "mode": "Ocean",
                "hasParts": true,
                "relation": null,
                "sub_mode": null,
                "major_mode": "Ocean",
                "is_multileg": false,
                "line_of_business": "inbound",
                "related_shipments": null,
                "stop_count_for_multistop": 2,
                "haul_away_tracking_window": "[\"2024-09-16 15:00:00\",\"2024-11-15 15:00:00\"]",
                "origin_arrived_at_received_ts": "2024-09-23T15:56:11.300232"
            },
            "origin_region": {
                "region": [
                    "EU"
                ]
            },
            "destination_region": {
                "region": [
                    "NA"
                ]
            },
            "shipment_stop_count": 2,
            "watched": false,
            "comments_count": null,
            "user_has_alert_me_subscription": false,
            "full_count": 2605,
            "current_location": {
                "current_city": null,
                "current_state": null,
                "current_country": "Ocean",
                "distance_progress": "null",
                "longitude": 0.3387,
                "latitude": 51.4534,
                "remaining_miles": null,
                "reported_at": "2024-09-24T03:00:00",
                "destination_eta": null,
                "updates": [
                    {
                        "time": "2024-09-24T03:00:00",
                        "longitude": 0.3387,
                        "latitude": 51.4534
                    }
                ]
            },
            "active_status_ng": "Active",
            "current_status_ng": "",
            "active_exceptions_ng": "Missed Drop-Off",
            "shipment_type_ng": "Inbound",
            "service_code": null,
            "on_time_percentage": null,
            "has_event_refs": false,
            "origin_location_code": "LNDN",
            "destination_location_code": "USNWK",
            "tracking_window_formatted": [
                "2024-09-16T15:00:00",
                "2024-11-15T15:00:00"
            ],
            "trailer_equipment_number": []
        },
        {
            "id": 39801661,
            "actor_type": "system",
            "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
            "actor_email": "test@freightverify-api.com",
            "fv_id": "FV9605085A",
            "created_by_org_id": 1004,
            "creator_shipment_id": "A498YBX9YP0",
            "total_distance": 3487.9233966392894,
            "progress": null,
            "status_updated_at": null,
            "obc_asset_id": "OCEAN-ASSET",
            "created_at": "2024-09-23T15:06:51.569303",
            "updated_at": "2024-09-23T15:06:57.370592",
            "is_accepted": null,
            "is_completed": null,
            "current_status": "FV_AUP",
            "active_status": "in_transit",
            "active_until": "2024-11-15T15:00:00",
            "eta": "2024-10-16T15:00:00",
            "current_exception": "missed_delivery_exceptions",
            "remaining_distance": null,
            "message_id": null,
            "is_behind_schedule": false,
            "picked_up_at": null,
            "delivered_at": null,
            "mode_id": 5,
            "leg": false,
            "mode_name": "Ocean",
            "trailer_number": null,
            "carrier_organization_id": 1003,
            "carrier_name": "TEST-Carrier",
            "carrier_fv_id": "FV0834338A",
            "carrier_mc_number": null,
            "carrier_scac": "TEST",
            "origin_code": "LNDN",
            "origin_name": "Port of London",
            "origin_location_id": 271418,
            "origin_location_actual_id": 18481377,
            "origin_address": "4988 Harbor Rd.",
            "origin_city": "Tilbury",
            "origin_state": "LND",
            "origin_postal_code": "SW15 5PU",
            "origin_country": "GB",
            "origin_lad_id": 19,
            "origin_lad_name": "Ocean Port",
            "origin_pickup_window": [
                1727103600.0,
                1727190000.0
            ],
            "origin_earliest_arrival": "2024-09-23T15:00:00",
            "origin_latest_arrival": "2024-09-24T15:00:00",
            "origin_distance": null,
            "origin_remaining_distance": null,
            "origin_calculated_eta": null,
            "origin_actual_arrival": "2024-09-24T03:00:00",
            "origin_actual_departure": null,
            "origin_stop_identifier": null,
            "destination_code": "USNWK",
            "destination_name": "Port Newark USNWK",
            "destination_location_id": 12253301,
            "destination_location_actual_id": 10767920,
            "destination_address": "3276 Industry Way",
            "destination_city": "Newark",
            "destination_state": "NJ ",
            "destination_postal_code": "07099",
            "destination_country": "US",
            "destination_lad_id": 29,
            "destination_lad_name": "Ocean Port",
            "destination_distance": null,
            "destination_remaining_distance": null,
            "destination_calculated_eta": "2024-10-16T15:00:00",
            "destination_actual_arrival": null,
            "destination_frozen_eta": null,
            "destination_frozen_eta_reason": null,
            "destination_actual_departure": null,
            "destination_stop_identifier": null,
            "destination_delivery_window": [
                1729004400.0,
                1729090800.0
            ],
            "destination_earliest_arrival": "2024-10-15T15:00:00",
            "destination_latest_arrival": "2024-10-16T15:00:00",
            "is_rack_return": false,
            "line_of_business_id": 2,
            "tracking_window": [
                1726498800.0,
                1731682800.0
            ],
            "tracking_disabled": null,
            "pro_number": "OCEAN-PRONUM",
            "rail_asset_id": null,
            "route_number": "OCEAN-ROUTE",
            "reference_number": null,
            "last_status_update": "2024-09-23T15:07:30.144388",
            "destination_eta": null,
            "current_city": null,
            "current_state": null,
            "remaining_miles": null,
            "current_country": "Ocean",
            "current_latitude": 51.4534,
            "current_longitude": 0.3387,
            "current_reported_at": "2024-10-16T15:00:00",
            "submode_id": null,
            "parent_shipment_id": null,
            "trip_plan_number": null,
            "current_road_organization_id": null,
            "current_road_name": null,
            "current_road_scac": null,
            "status_type_name": null,
            "status_name": null,
            "rail_train_id": null,
            "rail_loaded_status": null,
            "loaded_status": null,
            "shipment_reference_details": [
                {
                    "value": "29P20T5GL3",
                    "qualifier": "order_number",
                    "shipment_id": 39801661
                },
                {
                    "value": "OCEAN-PART1 (500)",
                    "qualifier": "part",
                    "shipment_id": 39801661
                },
                {
                    "value": "OCEAN-PART2 (2000)",
                    "qualifier": "part",
                    "shipment_id": 39801661
                },
                {
                    "value": "OCEAN-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39801661
                }
            ],
            "shipment_details": {
                "mode": "Ocean",
                "hasParts": true,
                "relation": null,
                "sub_mode": null,
                "major_mode": "Ocean",
                "is_multileg": false,
                "line_of_business": "inbound",
                "related_shipments": null,
                "stop_count_for_multistop": 2,
                "haul_away_tracking_window": "[\"2024-09-16 15:00:00\",\"2024-11-15 15:00:00\"]",
                "origin_arrived_at_received_ts": "2024-09-23T15:07:25.512336"
            },
            "origin_region": {
                "region": [
                    "EU"
                ]
            },
            "destination_region": {
                "region": [
                    "NA"
                ]
            },
            "shipment_stop_count": 2,
            "watched": false,
            "comments_count": null,
            "user_has_alert_me_subscription": false,
            "full_count": 2605,
            "current_location": {
                "current_city": null,
                "current_state": null,
                "current_country": "Ocean",
                "distance_progress": "null",
                "longitude": 0.3387,
                "latitude": 51.4534,
                "remaining_miles": null,
                "reported_at": "2024-10-16T15:00:00",
                "destination_eta": null,
                "updates": [
                    {
                        "time": "2024-10-16T15:00:00",
                        "longitude": 0.3387,
                        "latitude": 51.4534
                    }
                ]
            },
            "active_status_ng": "Active",
            "current_status_ng": "",
            "active_exceptions_ng": "Missed Drop-Off",
            "shipment_type_ng": "Inbound",
            "service_code": null,
            "on_time_percentage": null,
            "has_event_refs": false,
            "origin_location_code": "LNDN",
            "destination_location_code": "USNWK",
            "tracking_window_formatted": [
                "2024-09-16T15:00:00",
                "2024-11-15T15:00:00"
            ],
            "trailer_equipment_number": []
        },
        {
            "id": 39801667,
            "actor_type": "system",
            "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
            "actor_email": "test@freightverify-api.com",
            "fv_id": "FV3094013A",
            "created_by_org_id": 1004,
            "creator_shipment_id": "AVN4PTM8238",
            "total_distance": 3487.9233966392894,
            "progress": null,
            "status_updated_at": null,
            "obc_asset_id": "OCEAN-ASSET",
            "created_at": "2024-09-23T15:59:42.949229",
            "updated_at": "2024-09-23T15:59:48.162518",
            "is_accepted": null,
            "is_completed": null,
            "current_status": "FV_AUP",
            "active_status": "in_transit",
            "active_until": "2024-11-15T15:00:00",
            "eta": "2024-10-16T15:00:00",
            "current_exception": "missed_delivery_exceptions",
            "remaining_distance": null,
            "message_id": null,
            "is_behind_schedule": false,
            "picked_up_at": null,
            "delivered_at": null,
            "mode_id": 5,
            "leg": false,
            "mode_name": "Ocean",
            "trailer_number": null,
            "carrier_organization_id": 1003,
            "carrier_name": "TEST-Carrier",
            "carrier_fv_id": "FV0834338A",
            "carrier_mc_number": null,
            "carrier_scac": "TEST",
            "origin_code": "LNDN",
            "origin_name": "Port of London",
            "origin_location_id": 271418,
            "origin_location_actual_id": 18481377,
            "origin_address": "4988 Harbor Rd.",
            "origin_city": "Tilbury",
            "origin_state": "LND",
            "origin_postal_code": "SW15 5PU",
            "origin_country": "GB",
            "origin_lad_id": 19,
            "origin_lad_name": "Ocean Port",
            "origin_pickup_window": [
                1727103600.0,
                1727190000.0
            ],
            "origin_earliest_arrival": "2024-09-23T15:00:00",
            "origin_latest_arrival": "2024-09-24T15:00:00",
            "origin_distance": null,
            "origin_remaining_distance": null,
            "origin_calculated_eta": null,
            "origin_actual_arrival": "2024-09-24T03:00:00",
            "origin_actual_departure": null,
            "origin_stop_identifier": null,
            "destination_code": "USNWK",
            "destination_name": "Port Newark USNWK",
            "destination_location_id": 12253301,
            "destination_location_actual_id": 10767920,
            "destination_address": "3276 Industry Way",
            "destination_city": "Newark",
            "destination_state": "NJ ",
            "destination_postal_code": "07099",
            "destination_country": "US",
            "destination_lad_id": 29,
            "destination_lad_name": "Ocean Port",
            "destination_distance": null,
            "destination_remaining_distance": null,
            "destination_calculated_eta": "2024-10-16T15:00:00",
            "destination_actual_arrival": null,
            "destination_frozen_eta": null,
            "destination_frozen_eta_reason": null,
            "destination_actual_departure": null,
            "destination_stop_identifier": null,
            "destination_delivery_window": [
                1729004400.0,
                1729090800.0
            ],
            "destination_earliest_arrival": "2024-10-15T15:00:00",
            "destination_latest_arrival": "2024-10-16T15:00:00",
            "is_rack_return": false,
            "line_of_business_id": 2,
            "tracking_window": [
                1726498800.0,
                1731682800.0
            ],
            "tracking_disabled": null,
            "pro_number": "OCEAN-PRONUM",
            "rail_asset_id": null,
            "route_number": "OCEAN-ROUTE",
            "reference_number": null,
            "last_status_update": "2024-09-23T15:59:47.227826",
            "destination_eta": null,
            "current_city": null,
            "current_state": null,
            "remaining_miles": null,
            "current_country": "Ocean",
            "current_latitude": 51.4534,
            "current_longitude": 0.3387,
            "current_reported_at": "2024-09-24T03:00:00",
            "submode_id": null,
            "parent_shipment_id": null,
            "trip_plan_number": null,
            "current_road_organization_id": null,
            "current_road_name": null,
            "current_road_scac": null,
            "status_type_name": null,
            "status_name": null,
            "rail_train_id": null,
            "rail_loaded_status": null,
            "loaded_status": null,
            "shipment_reference_details": [
                {
                    "value": "BXWNPBDVNR",
                    "qualifier": "order_number",
                    "shipment_id": 39801667
                },
                {
                    "value": "OCEAN-PART1 (500)",
                    "qualifier": "part",
                    "shipment_id": 39801667
                },
                {
                    "value": "OCEAN-PART2 (2000)",
                    "qualifier": "part",
                    "shipment_id": 39801667
                },
                {
                    "value": "OCEAN-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39801667
                }
            ],
            "shipment_details": {
                "mode": "Ocean",
                "hasParts": true,
                "relation": null,
                "sub_mode": null,
                "major_mode": "Ocean",
                "is_multileg": false,
                "line_of_business": "inbound",
                "related_shipments": null,
                "stop_count_for_multistop": 2,
                "haul_away_tracking_window": "[\"2024-09-16 15:00:00\",\"2024-11-15 15:00:00\"]",
                "origin_arrived_at_received_ts": "2024-09-23T15:59:47.713832"
            },
            "origin_region": {
                "region": [
                    "EU"
                ]
            },
            "destination_region": {
                "region": [
                    "NA"
                ]
            },
            "shipment_stop_count": 2,
            "watched": false,
            "comments_count": null,
            "user_has_alert_me_subscription": false,
            "full_count": 2605,
            "current_location": {
                "current_city": null,
                "current_state": null,
                "current_country": "Ocean",
                "distance_progress": "null",
                "longitude": 0.3387,
                "latitude": 51.4534,
                "remaining_miles": null,
                "reported_at": "2024-09-24T03:00:00",
                "destination_eta": null,
                "updates": [
                    {
                        "time": "2024-09-24T03:00:00",
                        "longitude": 0.3387,
                        "latitude": 51.4534
                    }
                ]
            },
            "active_status_ng": "Active",
            "current_status_ng": "",
            "active_exceptions_ng": "Missed Drop-Off",
            "shipment_type_ng": "Inbound",
            "service_code": null,
            "on_time_percentage": null,
            "has_event_refs": false,
            "origin_location_code": "LNDN",
            "destination_location_code": "USNWK",
            "tracking_window_formatted": [
                "2024-09-16T15:00:00",
                "2024-11-15T15:00:00"
            ],
            "trailer_equipment_number": []
        },
        {
            "id": 39804244,
            "actor_type": "system",
            "actor_id": "auth0|5b9817c072d4bb47f9a5fae1",
            "actor_email": "test@freightverify-api.com",
            "fv_id": "FV8260915A",
            "created_by_org_id": 1004,
            "creator_shipment_id": "BK3XUBAC3UI",
            "total_distance": 3487.9233966392894,
            "progress": null,
            "status_updated_at": null,
            "obc_asset_id": null,
            "created_at": "2024-10-09T07:15:52.839171",
            "updated_at": "2024-10-09T07:15:55.191426",
            "is_accepted": null,
            "is_completed": null,
            "current_status": null,
            "active_status": "asset_pending",
            "active_until": "2024-11-17T06:30:00",
            "eta": "2024-10-18T06:30:00",
            "current_exception": "missed_delivery_exceptions",
            "remaining_distance": null,
            "message_id": null,
            "is_behind_schedule": false,
            "picked_up_at": null,
            "delivered_at": null,
            "mode_id": 5,
            "leg": false,
            "mode_name": "Ocean",
            "trailer_number": null,
            "carrier_organization_id": 1003,
            "carrier_name": "TEST-Carrier",
            "carrier_fv_id": "FV0834338A",
            "carrier_mc_number": null,
            "carrier_scac": "TEST",
            "origin_code": "LNDN",
            "origin_name": "Port of London",
            "origin_location_id": 271418,
            "origin_location_actual_id": 18481377,
            "origin_address": "4988 Harbor Rd.",
            "origin_city": "Tilbury",
            "origin_state": "LND",
            "origin_postal_code": "SW15 5PU",
            "origin_country": "GB",
            "origin_lad_id": 19,
            "origin_lad_name": "Ocean Port",
            "origin_pickup_window": [
                1727159400.0,
                1727245800.0
            ],
            "origin_earliest_arrival": "2024-09-24T06:30:00",
            "origin_latest_arrival": "2024-09-25T06:30:00",
            "origin_distance": null,
            "origin_remaining_distance": null,
            "origin_calculated_eta": null,
            "origin_actual_arrival": null,
            "origin_actual_departure": null,
            "origin_stop_identifier": null,
            "destination_code": "USNWK",
            "destination_name": "Port Newark USNWK",
            "destination_location_id": 12253301,
            "destination_location_actual_id": 10767920,
            "destination_address": "3276 Industry Way",
            "destination_city": "Newark",
            "destination_state": "NJ ",
            "destination_postal_code": "07099",
            "destination_country": "US",
            "destination_lad_id": 29,
            "destination_lad_name": "Ocean Port",
            "destination_distance": null,
            "destination_remaining_distance": null,
            "destination_calculated_eta": "2024-10-18T06:30:00",
            "destination_actual_arrival": null,
            "destination_frozen_eta": null,
            "destination_frozen_eta_reason": null,
            "destination_actual_departure": null,
            "destination_stop_identifier": null,
            "destination_delivery_window": [
                1729146600.0,
                1729233000.0
            ],
            "destination_earliest_arrival": "2024-10-17T06:30:00",
            "destination_latest_arrival": "2024-10-18T06:30:00",
            "is_rack_return": false,
            "line_of_business_id": 2,
            "tracking_window": [
                1726554600.0,
                1731825000.0
            ],
            "tracking_disabled": null,
            "pro_number": "OCEAN-PRONUM",
            "rail_asset_id": null,
            "route_number": "OCEAN-ROUTE",
            "reference_number": null,
            "last_status_update": null,
            "destination_eta": null,
            "current_city": null,
            "current_state": null,
            "remaining_miles": null,
            "current_country": null,
            "current_latitude": null,
            "current_longitude": null,
            "current_reported_at": null,
            "submode_id": null,
            "parent_shipment_id": null,
            "trip_plan_number": null,
            "current_road_organization_id": null,
            "current_road_name": null,
            "current_road_scac": null,
            "status_type_name": null,
            "status_name": null,
            "rail_train_id": null,
            "rail_loaded_status": null,
            "loaded_status": null,
            "shipment_reference_details": [
                {
                    "value": "Order1234",
                    "qualifier": "order_number",
                    "shipment_id": 39804244
                },
                {
                    "value": "OCEAN-PART1 (500)",
                    "qualifier": "part",
                    "shipment_id": 39804244
                },
                {
                    "value": "OCEAN-PART2 (2000)",
                    "qualifier": "part",
                    "shipment_id": 39804244
                },
                {
                    "value": "OCEAN-ROUTE",
                    "qualifier": "route_id",
                    "shipment_id": 39804244
                }
            ],
            "shipment_details": {
                "mode": "Ocean",
                "hasParts": true,
                "relation": null,
                "sub_mode": null,
                "major_mode": "Ocean",
                "is_multileg": false,
                "line_of_business": "inbound",
                "related_shipments": null,
                "haul_away_tracking_window": "[\"2024-09-17 06:30:00\",\"2024-11-17 06:30:00\"]"
            },
            "origin_region": {
                "region": [
                    "EU"
                ]
            },
            "destination_region": {
                "region": [
                    "NA"
                ]
            },
            "shipment_stop_count": 2,
            "watched": false,
            "comments_count": null,
            "user_has_alert_me_subscription": false,
            "full_count": 2605,
            "current_location": {
                "current_city": null,
                "current_state": null,
                "current_country": null,
                "distance_progress": "null",
                "longitude": null,
                "latitude": null,
                "remaining_miles": null,
                "reported_at": null,
                "destination_eta": null,
                "updates": []
            },
            "active_status_ng": "Pending: Asset ID",
            "current_status_ng": "",
            "active_exceptions_ng": "Missed Drop-Off",
            "shipment_type_ng": "Inbound",
            "service_code": null,
            "on_time_percentage": null,
            "has_event_refs": false,
            "origin_location_code": "LNDN",
            "destination_location_code": "USNWK",
            "tracking_window_formatted": [
                "2024-09-17T06:30:00",
                "2024-11-17T06:30:00"
            ],
            "trailer_equipment_number": []
        },
        {
            "id": 39805406,
            "actor_type": "system",
            "actor_id": "auth0|5b47a70bf3d20a5de664bdc9",
            "actor_email": "telematics@freightverify.com",
            "fv_id": "FV2787662A",
            "created_by_org_id": 1830,
            "creator_shipment_id": "QIJHH6QHLIC",
            "total_distance": 1496.3719782984792,
            "progress": 0,
            "status_updated_at": null,
            "obc_asset_id": "RAIL-ASSET",
            "created_at": "2024-10-14T17:24:34.808424",
            "updated_at": "2024-10-14T17:24:49.565205",
            "is_accepted": null,
            "is_completed": null,
            "current_status": null,
            "active_status": "in_transit",
            "active_until": "2024-11-15T08:00:00",
            "eta": "2024-11-23T01:00:00",
            "current_exception": null,
            "remaining_distance": 1496.3719782984792,
            "message_id": null,
            "is_behind_schedule": false,
            "picked_up_at": null,
            "delivered_at": null,
            "mode_id": 2,
            "leg": false,
            "mode_name": "Rail",
            "trailer_number": "RAIL-QIJHH6QHLIC",
            "carrier_organization_id": 1003,
            "carrier_name": "TEST-Carrier",
            "carrier_fv_id": "FV0834338A",
            "carrier_mc_number": null,
            "carrier_scac": "TEST",
            "origin_code": "566900000-2",
            "origin_name": "KC MIX CTR 2",
            "origin_location_id": 2610056,
            "origin_location_actual_id": 2610057,
            "origin_address": "KANSAS CITY",
            "origin_city": "KANSAS CITY",
            "origin_state": "MO ",
            "origin_postal_code": "64108",
            "origin_country": "US",
            "origin_lad_id": 12,
            "origin_lad_name": "Carrier Terminal",
            "origin_pickup_window": [
                1729123200.0,
                1729123200.0
            ],
            "origin_earliest_arrival": "2024-10-17T00:00:00",
            "origin_latest_arrival": "2024-10-17T00:00:00",
            "origin_distance": null,
            "origin_remaining_distance": null,
            "origin_calculated_eta": null,
            "origin_actual_arrival": "2024-10-15T02:00:00",
            "origin_actual_departure": "2024-10-15T23:00:00",
            "origin_stop_identifier": null,
            "destination_code": "762800000-2",
            "destination_name": "SLC MOTOR 2",
            "destination_location_id": 2610058,
            "destination_location_actual_id": 2610059,
            "destination_address": "SALT LAKE CITY",
            "destination_city": "SALT LAKE CITY",
            "destination_state": "UT ",
            "destination_postal_code": "84101",
            "destination_country": "US",
            "destination_lad_id": 12,
            "destination_lad_name": "Carrier Terminal",
            "destination_distance": null,
            "destination_remaining_distance": null,
            "destination_calculated_eta": "2024-11-23T01:00:00",
            "destination_actual_arrival": null,
            "destination_frozen_eta": null,
            "destination_frozen_eta_reason": null,
            "destination_actual_departure": null,
            "destination_stop_identifier": null,
            "destination_delivery_window": [
                1729843200.0,
                1729843200.0
            ],
            "destination_earliest_arrival": "2024-10-25T08:00:00",
            "destination_latest_arrival": "2024-10-25T08:00:00",
            "is_rack_return": false,
            "line_of_business_id": 2,
            "tracking_window": [
                1728924900.0,
                1731657600.0
            ],
            "tracking_disabled": null,
            "pro_number": "4Y7VHGMWXP",
            "rail_asset_id": "RAIL-ASSET",
            "route_number": "SHIPPER2-RAIL-ROUTE",
            "reference_number": null,
            "last_status_update": "2024-10-14T17:24:58.648267",
            "destination_eta": "2024-10-27T01:00:00",
            "current_city": null,
            "current_state": null,
            "remaining_miles": null,
            "current_country": null,
            "current_latitude": 39.11944,
            "current_longitude": -94.58896,
            "current_reported_at": "2024-10-16T01:00:00",
            "submode_id": null,
            "parent_shipment_id": null,
            "trip_plan_number": "12345-4",
            "current_road_organization_id": null,
            "current_road_name": null,
            "current_road_scac": null,
            "status_type_name": null,
            "status_name": null,
            "rail_train_id": null,
            "rail_loaded_status": null,
            "loaded_status": null,
            "shipment_reference_details": [
                {
                    "value": "1KE97583",
                    "qualifier": "BM",
                    "shipment_id": 39805406
                },
                {
                    "value": "RAIL-QIJHH6QHLIC",
                    "qualifier": "equipment_number",
                    "shipment_id": 39805406
                },
                {
                    "value": "Order1234",
                    "qualifier": "order_number",
                    "shipment_id": 39805406
                }
            ],
            "shipment_details": {
                "mode": "Rail",
                "l1_eta": "2024-10-26T23:00:00+00:00",
                "relation": null,
                "sub_mode": null,
                "major_mode": "Rail",
                "sync_types": [
                    "Equipment"
                ],
                "is_multileg": false,
                "is_off_route": true,
                "line_of_business": "inbound",
                "related_shipments": null,
                "daily_eta_extension_ts": "2024-11-10T19:57:18Z",
                "stop_count_for_multistop": 3,
                "haul_away_tracking_window": "[\"2024-10-14 16:55:00\",\"2024-11-15 08:00:00\"]"
            },
            "origin_region": {
                "region": [
                    "NA"
                ]
            },
            "destination_region": {
                "region": [
                    "NA"
                ]
            },
            "shipment_stop_count": 3,
            "watched": false,
            "comments_count": null,
            "user_has_alert_me_subscription": false,
            "full_count": 2605,
            "current_location": {
                "current_city": null,
                "current_state": null,
                "current_country": null,
                "distance_progress": "0%",
                "longitude": -94.58896,
                "latitude": 39.11944,
                "remaining_miles": null,
                "reported_at": "2024-10-16T01:00:00",
                "destination_eta": "2024-10-27T01:00:00",
                "updates": [
                    {
                        "time": "2024-10-16T01:00:00",
                        "longitude": -94.58896,
                        "latitude": 39.11944
                    }
                ]
            },
            "active_status_ng": "Active",
            "current_status_ng": "",
            "active_exceptions_ng": "",
            "shipment_type_ng": "Inbound",
            "service_code": null,
            "on_time_percentage": null,
            "has_event_refs": false,
            "origin_location_code": "566900000-2",
            "destination_location_code": "762800000-2",
            "tracking_window_formatted": [
                "2024-10-14T16:55:00",
                "2024-11-15T08:00:00"
            ],
            "trailer_equipment_number": [
                "RAIL-QIJHH6QHLIC"
            ]
        },
        {
            "id": 39805787,
            "actor_type": "system",
            "actor_id": "auth0|5b47a70bf3d20a5de664bdc9",
            "actor_email": "telematics@freightverify.com",
            "fv_id": "FV6771814A",
            "created_by_org_id": 1004,
            "creator_shipment_id": "AAZKR7E22YG",
            "total_distance": 922.8192163154054,
            "progress": 0,
            "status_updated_at": null,
            "obc_asset_id": "RAIL-ASSET",
            "created_at": "2024-10-15T20:37:27.630318",
            "updated_at": "2024-10-15T20:37:39.966325",
            "is_accepted": null,
            "is_completed": null,
            "current_status": null,
            "active_status": "in_transit",
            "active_until": "2024-11-15T22:00:00",
            "eta": "2024-11-23T02:30:00",
            "current_exception": "behind_schedule",
            "remaining_distance": 922.8192163154054,
            "message_id": null,
            "is_behind_schedule": true,
            "picked_up_at": null,
            "delivered_at": null,
            "mode_id": 2,
            "leg": false,
            "mode_name": "Rail",
            "trailer_number": "RAIL-AAZKR7E22YG",
            "carrier_organization_id": 1003,
            "carrier_name": "TEST-Carrier",
            "carrier_fv_id": "FV0834338A",
            "carrier_mc_number": null,
            "carrier_scac": "TEST",
            "origin_code": "566900000-1",
            "origin_name": "FORD MOTOR MIX CTR",
            "origin_location_id": 212569,
            "origin_location_actual_id": 765444,
            "origin_address": "KANSAS CITY",
            "origin_city": "KANSAS CITY",
            "origin_state": "MO ",
            "origin_postal_code": "64108",
            "origin_country": "US",
            "origin_lad_id": 12,
            "origin_lad_name": "Carrier Terminal",
            "origin_pickup_window": [
                1729022400.0,
                1729022400.0
            ],
            "origin_earliest_arrival": "2024-10-15T20:00:00",
            "origin_latest_arrival": "2024-10-15T20:00:00",
            "origin_distance": null,
            "origin_remaining_distance": null,
            "origin_calculated_eta": null,
            "origin_actual_arrival": "2024-10-15T20:00:00",
            "origin_actual_departure": "2024-10-15T22:00:00",
            "origin_stop_identifier": null,
            "destination_code": "762800000-1",
            "destination_name": "FORD MOTOR",
            "destination_location_id": 212571,
            "destination_location_actual_id": 765445,
            "destination_address": "SALT LAKE CITY",
            "destination_city": "SALT LAKE CITY",
            "destination_state": "UT ",
            "destination_postal_code": "84101",
            "destination_country": "US",
            "destination_lad_id": 12,
            "destination_lad_name": "Carrier Terminal",
            "destination_distance": null,
            "destination_remaining_distance": null,
            "destination_calculated_eta": "2024-11-23T02:30:00",
            "destination_actual_arrival": null,
            "destination_frozen_eta": null,
            "destination_frozen_eta_reason": null,
            "destination_actual_departure": null,
            "destination_stop_identifier": null,
            "destination_delivery_window": [
                1729893600.0,
                1729893600.0
            ],
            "destination_earliest_arrival": "2024-10-25T22:00:00",
            "destination_latest_arrival": "2024-10-25T22:00:00",
            "is_rack_return": false,
            "line_of_business_id": 2,
            "tracking_window": [
                1729020600.0,
                1731708000.0
            ],
            "tracking_disabled": null,
            "pro_number": "LL8KU8BTWE",
            "rail_asset_id": "RAIL-ASSET",
            "route_number": null,
            "reference_number": null,
            "last_status_update": "2024-10-15T20:37:39.323779",
            "destination_eta": "2024-10-28T02:30:00",
            "current_city": null,
            "current_state": null,
            "remaining_miles": null,
            "current_country": null,
            "current_latitude": 39.11944,
            "current_longitude": -94.58896,
            "current_reported_at": "2024-10-15T22:00:00",
            "submode_id": null,
            "parent_shipment_id": null,
            "trip_plan_number": null,
            "current_road_organization_id": null,
            "current_road_name": null,
            "current_road_scac": null,
            "status_type_name": null,
            "status_name": null,
            "rail_train_id": "RAIL-TRAIN",
            "rail_loaded_status": "L",
            "loaded_status": "L",
            "shipment_reference_details": [
                {
                    "value": "1KE97583",
                    "qualifier": "BM",
                    "shipment_id": 39805787
                },
                {
                    "value": "RAIL-AAZKR7E22YG",
                    "qualifier": "equipment_number",
                    "shipment_id": 39805787
                },
                {
                    "value": "BXWNPBDVNR",
                    "qualifier": "order_number",
                    "shipment_id": 39805787
                }
            ],
            "shipment_details": {
                "mode": "Rail",
                "l1_eta": "2024-10-28T02:30:00+00:00",
                "relation": null,
                "sub_mode": null,
                "major_mode": "Rail",
                "sync_types": [
                    "Equipment"
                ],
                "is_multileg": false,
                "line_of_business": "inbound",
                "related_shipments": null,
                "daily_eta_extension_ts": "2024-11-10T21:57:18Z",
                "stop_count_for_multistop": 2,
                "haul_away_tracking_window": "[\"2024-10-15 19:30:00\",\"2024-11-15 22:00:00\"]"
            },
            "origin_region": {
                "region": [
                    "NA"
                ]
            },
            "destination_region": {
                "region": [
                    "NA"
                ]
            },
            "shipment_stop_count": 2,
            "watched": false,
            "comments_count": null,
            "user_has_alert_me_subscription": false,
            "full_count": 2605,
            "current_location": {
                "current_city": null,
                "current_state": null,
                "current_country": null,
                "distance_progress": "0%",
                "longitude": -94.58896,
                "latitude": 39.11944,
                "remaining_miles": null,
                "reported_at": "2024-10-15T22:00:00",
                "destination_eta": "2024-10-28T02:30:00",
                "updates": [
                    {
                        "time": "2024-10-15T22:00:00",
                        "longitude": -94.58896,
                        "latitude": 39.11944
                    }
                ]
            },
            "active_status_ng": "Active",
            "current_status_ng": "",
            "active_exceptions_ng": "Behind Schedule",
            "shipment_type_ng": "Inbound",
            "service_code": null,
            "on_time_percentage": null,
            "has_event_refs": false,
            "origin_location_code": "566900000-1",
            "destination_location_code": "762800000-1",
            "tracking_window_formatted": [
                "2024-10-15T19:30:00",
                "2024-11-15T22:00:00"
            ],
            "trailer_equipment_number": [
                "RAIL-AAZKR7E22YG"
            ]
        },
        {
            "id": 39805790,
            "actor_type": "system",
            "actor_id": "auth0|5b47a70bf3d20a5de664bdc9",
            "actor_email": "telematics@freightverify.com",
            "fv_id": "FV3115554A",
            "created_by_org_id": 1004,
            "creator_shipment_id": "ASQ1S9VGGXU",
            "total_distance": 922.8192163154054,
            "progress": 0,
            "status_updated_at": null,
            "obc_asset_id": "RAIL-ASSET",
            "created_at": "2024-10-15T21:14:41.729184",
            "updated_at": "2024-10-15T21:15:05.337816",
            "is_accepted": null,
            "is_completed": null,
            "current_status": null,
            "active_status": "in_transit",
            "active_until": "2024-11-15T23:00:00",
            "eta": "2024-11-23T02:30:00",
            "current_exception": "behind_schedule",
            "remaining_distance": 922.8192163154054,
            "message_id": null,
            "is_behind_schedule": true,
            "picked_up_at": null,
            "delivered_at": null,
            "mode_id": 2,
            "leg": false,
            "mode_name": "Rail",
            "trailer_number": "RAIL-ASQ1S9VGGXU",
            "carrier_organization_id": 1003,
            "carrier_name": "TEST-Carrier",
            "carrier_fv_id": "FV0834338A",
            "carrier_mc_number": null,
            "carrier_scac": "TEST",
            "origin_code": "566900000-1",
            "origin_name": "FORD MOTOR MIX CTR",
            "origin_location_id": 212569,
            "origin_location_actual_id": 765444,
            "origin_address": "KANSAS CITY",
            "origin_city": "KANSAS CITY",
            "origin_state": "MO ",
            "origin_postal_code": "64108",
            "origin_country": "US",
            "origin_lad_id": 12,
            "origin_lad_name": "Carrier Terminal",
            "origin_pickup_window": [
                1729026000.0,
                1729026000.0
            ],
            "origin_earliest_arrival": "2024-10-15T21:00:00",
            "origin_latest_arrival": "2024-10-15T21:00:00",
            "origin_distance": null,
            "origin_remaining_distance": null,
            "origin_calculated_eta": null,
            "origin_actual_arrival": "2024-10-15T21:00:00",
            "origin_actual_departure": null,
            "origin_stop_identifier": null,
            "destination_code": "762800000-1",
            "destination_name": "FORD MOTOR",
            "destination_location_id": 212571,
            "destination_location_actual_id": 765445,
            "destination_address": "SALT LAKE CITY",
            "destination_city": "SALT LAKE CITY",
            "destination_state": "UT ",
            "destination_postal_code": "84101",
            "destination_country": "US",
            "destination_lad_id": 12,
            "destination_lad_name": "Carrier Terminal",
            "destination_distance": null,
            "destination_remaining_distance": null,
            "destination_calculated_eta": "2024-11-23T02:30:00",
            "destination_actual_arrival": null,
            "destination_frozen_eta": null,
            "destination_frozen_eta_reason": null,
            "destination_actual_departure": null,
            "destination_stop_identifier": null,
            "destination_delivery_window": [
                1729897200.0,
                1729897200.0
            ],
            "destination_earliest_arrival": "2024-10-25T23:00:00",
            "destination_latest_arrival": "2024-10-25T23:00:00",
            "is_rack_return": false,
            "line_of_business_id": 2,
            "tracking_window": [
                1729024200.0,
                1731711600.0
            ],
            "tracking_disabled": null,
            "pro_number": "PPHVAD3END",
            "rail_asset_id": "RAIL-ASSET",
            "route_number": null,
            "reference_number": null,
            "last_status_update": "2024-10-15T21:14:58.478322",
            "destination_eta": "2024-10-28T02:30:00",
            "current_city": null,
            "current_state": null,
            "remaining_miles": null,
            "current_country": null,
            "current_latitude": 39.11944,
            "current_longitude": -94.58896,
            "current_reported_at": "2024-10-15T23:00:00",
            "submode_id": null,
            "parent_shipment_id": null,
            "trip_plan_number": null,
            "current_road_organization_id": null,
            "current_road_name": null,
            "current_road_scac": null,
            "status_type_name": null,
            "status_name": null,
            "rail_train_id": "RAIL-TRAIN",
            "rail_loaded_status": "L",
            "loaded_status": "L",
            "shipment_reference_details": [
                {
                    "value": "1KE97583",
                    "qualifier": "BM",
                    "shipment_id": 39805790
                },
                {
                    "value": "RAIL-ASQ1S9VGGXU",
                    "qualifier": "equipment_number",
                    "shipment_id": 39805790
                },
                {
                    "value": "BXWNPBDVNR",
                    "qualifier": "order_number",
                    "shipment_id": 39805790
                }
            ],
            "shipment_details": {
                "mode": "Rail",
                "l1_eta": "2024-10-28T02:30:00+00:00",
                "relation": null,
                "sub_mode": null,
                "major_mode": "Rail",
                "sync_types": [
                    "Equipment"
                ],
                "is_multileg": false,
                "line_of_business": "inbound",
                "related_shipments": null,
                "daily_eta_extension_ts": "2024-11-10T22:57:17Z",
                "stop_count_for_multistop": 2,
                "haul_away_tracking_window": "[\"2024-10-15 20:30:00\",\"2024-11-15 23:00:00\"]"
            },
            "origin_region": {
                "region": [
                    "NA"
                ]
            },
            "destination_region": {
                "region": [
                    "NA"
                ]
            },
            "shipment_stop_count": 2,
            "watched": false,
            "comments_count": null,
            "user_has_alert_me_subscription": false,
            "full_count": 2605,
            "current_location": {
                "current_city": null,
                "current_state": null,
                "current_country": null,
                "distance_progress": "0%",
                "longitude": -94.58896,
                "latitude": 39.11944,
                "remaining_miles": null,
                "reported_at": "2024-10-15T23:00:00",
                "destination_eta": "2024-10-28T02:30:00",
                "updates": [
                    {
                        "time": "2024-10-15T23:00:00",
                        "longitude": -94.58896,
                        "latitude": 39.11944
                    }
                ]
            },
            "active_status_ng": "Active",
            "current_status_ng": "",
            "active_exceptions_ng": "Behind Schedule",
            "shipment_type_ng": "Inbound",
            "service_code": null,
            "on_time_percentage": null,
            "has_event_refs": false,
            "origin_location_code": "566900000-1",
            "destination_location_code": "762800000-1",
            "tracking_window_formatted": [
                "2024-10-15T20:30:00",
                "2024-11-15T23:00:00"
            ],
            "trailer_equipment_number": [
                "RAIL-ASQ1S9VGGXU"
            ]
        }
    ]
}
