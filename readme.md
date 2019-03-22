Canjun Navy Processes
=======================

## Dependencies
This project depends on both rules and a model.
- The rules can be found [here ](https://github.com/NAPS-emergency-response-project/cajun-navy-rules/tree/justin) (the justin branch)
- The model can be found [here](https://github.com/NAPS-emergency-response-project/cajun-navy-rules-model).

## Running the Reproducer

The process to test the rules is the `Reproducer.bpmn2` process with id `src.Reproducer`.

JSON input for `src.Reproducer`:

    {
        "incident": {
            "com.redhat.cajun.navy.rules.model.Incident": {
                "id": 1,
                "latitude": 34.16877,
                "longitude": -77.87045,
                "numberOfPeople": 2,
                "isMedicalNeeded": true,
                "victimName": "Justin",
                "victimPhoneNumber": "123-456-7890"
            }
        },
        "responders": {
            "com.redhat.cajun.navy.rules.model.Responders": {
                "responders": [
                    {
                        "fullname": "full name",
                        "hasMission": false,
                        "boatCapacity": 2,
                        "longitude": "-77.87045",
                        "hasMedical": false,
                        "phoneNumber": "555-555-5555",
                        "latitude": "34.16877",
                        "isAvailable": true,
                        "id": 1
                    },
                    {
                        "fullname": "full name",
                        "hasMission": false,
                        "boatCapacity": 4,
                        "longitude": "-77.8718",
                        "hasMedical": true,
                        "phoneNumber": "555-555-5555",
                        "latitude": "34.23519",
                        "isAvailable": true,
                        "id": 2
                    },
                    {
                        "fullname": "full name",
                        "hasMission": false,
                        "boatCapacity": 6,
                        "longitude": "-77.81316",
                        "hasMedical": false,
                        "phoneNumber": "555-555-5555",
                        "latitude": "34.11331",
                        "isAvailable": true,
                        "id": 3
                    },
                    {
                        "fullname": "full name",
                        "hasMission": false,
                        "boatCapacity": 8,
                        "longitude": "-77.86253",
                        "hasMedical": true,
                        "phoneNumber": "555-555-5555",
                        "latitude": "34.19219",
                        "isAvailable": true,
                        "id": 4
                    }
                ]
            }
        }
    }
