# Intercom Server Tag

This tag allows you to send information to your Intercom.

With this tag, you can : 

- Create or update a User
- Create or update a Company
- Send data event from a User

## How do I use this tag?

To use this tag, you must have an Intercom app. You can create one by going here: https://app.intercom.com/a/apps/vnkbkvuc/developer-hub.

With this, you should have an Access Token (available in the Authentication page in the App). This is what you will use in the tag under the variable "Access Token".

After that, in the tag you can choose what data to send.

### Creating/Updating a Company

You must provide your internal company id. This is what Intercom will use to know if it needs to create the company, or simply update it.
You can choose to only send partial data, and it will only update the corresponding data.

You can also send custom attributes for a Company, that will be automatically created in Intercom.


### Creating/Updating a User

For this entity, either Email or UserId is required for the creation or update. The user id is your internal user id.

You can also send custom attributes for a User, that will be automatically created in Intercom.

### Submit Event

To submit an Event to Intercom, you either need to have the userid, or the email.
Events are information on what Users did and when they did it. For example, the first time they subscribed to a paid plan, or the most recent time they changed their plan would be represented by events.

With DataEvent, you can submit up to 10 optional metadata.

More information in the dataevent in the Intercom developer documentation: https://developers.intercom.com/intercom-api-reference/v1.4/reference#events
