# TrackTogether data

TrackTogether is a non-profit supporting the NHS and Her Majesty’s Government to manage the COVID-19 crisis by providing data. The tracker (www.tracktogether.org) asks people to complete a simple survey (30 seconds long) about their symptoms.

## Data descriptions

| Key               | Values                | Question(s) asked                                                                                                                                                                                                        | Available from                                                 |
| ----------------- | --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------- |
| fever             | Boolean               | Have you experienced a high temperature – this means you feel hot to touch on your chest or back (you do not need to measure your temperature) – since 1st March?                                                        | 21 March 2020 at 20:41:21 GMT                                  |
| cough             | Boolean               | Have you experienced a new, continuous cough? – this means coughing a lot for more than an hour, or 3 or more coughing episodes in 24 hours (if you usually have a cough, it may be worse than usual) – since 1st March? | 21 March 2020 at 20:41:21 GMT                                  |
| isolation         | Boolean               | Are you currently self-isolating or have you self-isolated (stayed indoors and avoided contact with those outside your household)?                                                                                       | 21 March 2020 at 20:41:21 GMT                                  |
| age               | Number                | What is your age?                                                                                                                                                                                                        | 21 March 2020 at 20:41:21 GMT                                  |
| senses            | Boolean               | Have you experienced a loss of sense and smell and taste – not yet confirmed as a common symptom, though anecdotal evidence suggests it may be – since 1st March?                                                        | 22 March 2020 at 20:20:57 GMT to 26 March 2020 at 23:32:50 GMT |
| tested            | Boolean               | Have you been tested for COVID-19?                                                                                                                                                                                       | 23 March 2020 at 10:20:45 GMT                                  |
| testedPositive    | Boolean               | If yes, did you test positive for COVID-19? Ignore if not tested                                                                                                                                                         | 23 March 2020 at 10:20:45 GMT                                  |
| country           | String (Country name) | In which country do you live?                                                                                                                                                                                            | 23 March 2020 at 17:32:36 GMT                                  |
| isolationReason   | Detailed Below        | Why are you self-isolating/staying at home?                                                                                                                                                                              | 25 March 2020 at 20:54:03 GMT                                  |
| feverRecorded     | Detailed Below        | If you have a thermometer, and can measure your fever, please record the value here                                                                                                                                      | 26 March 2020 at 23:32:50 GMT                                  |
| pressure          | Boolean               | Do you have pain or pressure in your chest?                                                                                                                                                                              | 26 March 2020 at 23:32:50 GMT                                  |
| confused          | Boolean               | Do you feel confused (or if you are answering this on someone else’s behalf, are they difficult to arouse)?                                                                                                              | 26 March 2020 at 23:32:50 GMT                                  |
| blueLips          | Boolean               | Is your face or are your lips blue in colour?                                                                                                                                                                            | 26 March 2020 at 23:32:50 GMT                                  |
| shortnessOfBreath | Boolean               | Do you have shortness of breath?                                                                                                                                                                                         | 26 March 2020 at 23:32:50 GMT                                  |

### isolationReason

Asked as a multi-select box, stored as a JSON object, if the key exists, the option was selected

| Key             | Question(s) asked                |
| --------------- | -------------------------------- |
| showingSymptoms | I have had symptoms              |
| highRiskGroup   | I am in a high risk group        |
| government      | I am following government advice |
| notIsolating    | I am not self-isolating          |

### feverRecorded

Asked as a multi-part question (number input for “temperature”, drop down selector [C, F] for “measure”, stored as a JSON object, with default value `{ temperature: 0, measure: “C” }`

## Future data

We will be continuously updating this dataset as it comes in from the tracktogether.org survey

## Contributing

Please contact rasheed@tracktogether.org for collaboration opportunities.

## License

[CC](https://choosealicense.com/licenses/cc0-1.0/)
