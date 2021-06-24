# Prototype-To-Demonstrate-The-Advantages-Of-Using-A-Digital-Transcriber-In-A-Business-Environment
Co-Created with sujithksam92

Communication is a big issue in today's world. In a survey of 400 companies, an average loss of $62.4 million per year was recorded due to miscommunication. This can be attributed to various different issues in the workforce, the work environment or the communications channels. Businesses have diverse ways of running their day to day communications. Depending on the type of business, there are varying communication protocols affected by the size of the business, scale, diversity, hierarchy etc. For example, a software product business might be using Agile as it's development methodology. There is a need for strong communication channels between multi-disciplinary teams, probably located in different geographies, to be established for this kind of methodologies to be effective. This calls for detailed documentation, frequent communication and a lot of cooperation in the system. The need to have a human resource to ensure that communications are in place, that everyone knows about the deliverables and proceedings in their projects, is quite redundant. Further, this is not the most optimal way of doing things.

 The solution we propose takes into account the growing popularity of speech recognition and text analysis. Speech recognition is estimated to grow into a $4.9 Billion market. There are multiple applications for this technology. We have used AWS services and Python to build a simple prototype to demonstrate how speech analytics powered smart agents can be deployed on collaboration tools like Slack, to integrate with the native work environment and help transcribe, analyse and interpret human voice that's exchanged in conversations.
To demonstrate, we've picked the following 3 different scenes from movies/shows and extracted their audio tracks: 1) The conversation between Leonardo DiCaprio & Matthew McConaughey in 'The Wolf Of Wall Street' 2) An argument between two people in 'Angry Dinner' 3) Matthew McConaughey's Oscar speech on winning the Best Actor

After having all of these put up on AWS S3 buckets, we invoke the Transcribe method for Speech-To-Text conversion and then the resulting JSON is what we use to run sentiment analysis powered by AWS. The final outcome of the code snippet identifies the predominant sentiment of the audio file and posts a summary to Slack with Slack RTM API. The core idea to take home from here is that, an entire meeting's audio can be used by an agent of this sort to identify the criticality/non-criticality of the matters discussed, automate the notifications rolled out to the different teams and even the future probability of building a method to condense the bulk of discussions into just actionable insights with minimal human intervention.

This prototype can be flushed out to more detail and to have more functionalities including deploying an Alexa powered device in the workflow, using a dictionary to better interpret structure and nature of the conversations. The is also room to use a purpose built Neural Network like the DeepSpeech.
