# alexa-hosted-workshop-edd19

## Skill
* Creamos un nuevo skill en es_ES, custom y con Alexa-Hosted
* [Interactor model](https://gist.github.com/kinisoftware/0f99d7c689d257f05f330a0f4189c65c)

## Lambda
* [Talks repository](https://gist.github.com/kinisoftware/57bb77e3f2f8070f0247aa0d7c6aac1a)
* [Interceptors](https://gist.github.com/kinisoftware/bfa5732cbf83f09206c792b5e1c5ea1b)
* [Index](https://gist.github.com/kinisoftware/1e18c7277e090019fd085e14f26dbc6e)

## Workshop steps
* Create a developer account > https://developer.amazon.com/alexa/console/ask
* Create custom skill with Alexa-Hosted (Node.js) option
* Check Interactor model (Build tab):
  * Check invocation name
  * Delete HelloWordlIntent
  * Add intent: 'ScheduleIntent'
  * Add a couple of sample utterances:
    * 'que charlas hay a las once y media'
    * 'quer charlas hay sobre negocio'
  * Identify slots
    * slotTime > AMAZON.TIME
    * talkTopic > Create a custom slot 'TalkTopicType' (next step)
  * Create a custom slot 'TalkTopicType'
    * Add values/id/synonyms from example interactor model
  * Add more sample utterances from example interactor model to ScheduleIntent
  * Test the interactor model with 'Evaluate Model' tool
* Check Server code (Code tab):
  * Delete index.js
  * Check & customize package.json file
  * Create file for talks repository > Copy from link
  * Create file index.js
    * Copy skill builder code and delete the line for the ScheduleIntentHandler
    * Copy interceptors code
    * Copy launch request handler
    * Copy amazon predefined intent handlers
    * Copy error handler
  * Test the skill (Test tab)
  * Add the ScheduleIntentHandler
  * Add SSML to talk's title
  * Check logs
* Check Test tab
* Check Distribution tab
* Check Certification tab
* Check Analytics tab
    
  
  
  
  



