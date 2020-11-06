# XApi Profile
This page describes to xAPI statement components that can be used when working with xAPI.

## Verbs

Name | IRI | Used With | Common Attributes | Description
--|--|--|--|--|
Intialized | http://adlnet.gov/expapi/verbs/initialized |  |  | Initialized the application
Terminated | http://adlnet.gov/expapi/verbs/terminated |  |  | Terminated the application
Session Start | http://adlnet.gov/expapi/verbs/launched |  |  | Session started
Focused | http://id.tincanapi.com/verb/focused |  |  | Indicates that a user has focused on a target object. This is the opposite of 'unfocused'. For example, it indicates that the user has clicked to focus or regain focus on the application, content or activity.
Unfocused | http://id.tincanapi.com/verb/focused |  |  | Indicates that the user has lost focus of the target object. For example, this could be used when the user clicks outside a given application, window or activity.
Donned | http://xapiprofile.org/xapi/verbs/donned | Real-word objects |  | The user has put on an object, like a hat or a VR headset.
Doffed | http://xapiprofile.org/xapi/verbs/donned | Real-world objects |  | The user has taken an object off, like a hat or a VR headset.
Teleported | https://xapiprofile.org/xapi/verbs/teleported |  |  | The user has instanteously moved from one position to another.
Grabbed | https://xapiprofle.org/xapi/verbs/grabbed |  |  | The user has grabbed a virtual object and is holding it
Released | https://w3id.org/xapi/dod-isd/verbs/released |  |  | Allow something to move, act, or flow freely.
Pressed | https://xapiprofile.org/xapi/verbs/pressed |  |  | Move or cause to move into a position of contact with something by exerting continuous physical force.
Selected | http://id.tincanapi.com/verb/selected |  |  | Indicates that the actor selects an object from a collection or set to use it in an activity. The collection would be the context parent element.
Interacted | http://adlnet.gov/expapi/verbs/interacted | World Objects |  | User interacted with an object.
Used Object | https://xapiprofile.org/xapi/verbs/used | World Objects |  | User used an object (potentially on another object)
End Touch | https://xapiprofile.org/xapi/verbs/touched | World Objects | duration, completed | User stopped touching an object.
End Gaze | https://xapiprofile.org/xapi/verbs/gazed | World Objects | duration, completed | User stopped gazing at an object
Start Place | https://xapiprofile.org/xapi/verbs/placed | World Objects |  | User placed an object in / on another object
End Place | https://xapiprofile.org/xapi/verbs/placed | World Objects | duration, completed | User stopped placing an object on/in another object (moved it out of the vicinity to qualify as "placing")
Equip | https://xapiprofile.org/xapi/verbs/equipped | World Objects | completed | User equipped an object (article of clothing, etc.) on a part of their body
Unequip | https://xapiprofile.org/xapi/verbs/unequipped | World Objects | completed | User removed a previously equipped object
End Point At | https://xapiprofile.org/xapi/verbs/selected | World Objects | duration, completed | User ended pointing at an object with a hand controller
Spoke | https://xapiprofile.org/xapi/verbs/spoke |  |  | User initiated an action by speaking
Heard | https://xapiprofile.org/xapi/verbs/heard | Character Dialog |  | Character spoke to the user

## Objects

Name | IRI | Used With | Common Attributes | Description
--|--|--|--|--|
Head Mounted Display | https://xapiprofile.org/xapi/activites/hmd-device |  |  | A device that the user wears on their head that has a graphical display in front of one or more eyes.
Area | https://w3id.org/xapi/seriousgames/activity-types/area |  |  | An identified area inside the game world. In some games they can also be worlds. Represents an aggregation of zones.
Scenario | http://id.tincanapi.com/activitytype/scenario |  |  | Maps to a learning module, a well-defined learning scenario with measured outcomes.
Playable Content | http://xapiprofile.org/xapi/activities/motive.ui.playableContent |  |  | Content (messages, audio, video, etc.) with a defined beginning and end. Users can often "close" this content through a UI mechanism.
Guide Content | http://xapiprofile.org/xapi/activities/motive.ui.guideContent |  |  | Content that provides guides for how to complete a task, for example. Not user controlled, lifetime is managed by the authoring tool.
Conversation | http://xapiprofile.org/xapi/activities/motive.ai.conversation |  |  | User conversed with one or more characters in the scene using AI or other mechanism.
World Object | http://xapiprofile.org/xapi/activities/motive.3d.worldObject |  |  | Represents a virtual object

## Extensions / Values

Name | IRI | Used With | Common Attributes | Description
--|--|--|--|--|
Position | http://id.tincanapi.com/extension/position |  |  | Represents the position of the object in a group or collection of elements. It is needed when the group of elements should be in order.
Rotation | https://xapiprofile.org/xapi/extensions/rotation |  |  | Represents the rotation of an object in space
Device Info | https://xapiprofile.org/xapi/extensions/device-info |  |  | Series of values that lists information about a device that the current user is using
Distance | http://id.tincanapi.com/extension/measurement |  |  | Value that represents a measured unit or physical quantity such as a distance or weight. For interoperability the value should be a string that follows the SI (International System of Units) recommendations for formatting and may include any value that can be described by its units. For additional information see the ISO 80000 standard.
Duration | http://id.tincanapi.com/extension/duration |  |  | Value representing a length of time, for example the length of a video.
Starting Position | http://id.tincanapi.com/extension/starting-position |  |  | Initial position within an ordinal set of numbers. Can also be thought of as a rank. For example the starting position of a car or runner in a race. To be used with 'Ending Position.'
Ending Position | http://id.tincanapi.com/extension/ending-position |  |  | Final position within an ordinal set of numbers. Can also be thought of as a rank. For example the ending position of a car or runner in a race. To be used with Starting Position.
Velocity | https://xapiprofile.org/xapi/extensions/velocity |  |  | The speed of an object in space
