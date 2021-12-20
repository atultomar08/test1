**DISCLAIMER**

:warning: The information shared in the document is in regards to iOS application however the topic is relevant for all platforms including android and web.

## Introduction and table of contents

Accessibility, also referred to as inclusivity is all about making the app work for as wide a range of people as possible. That can include the very young, the very old, people brand new to computers and mobile devices, and also people with disabilities and special needs. This topic often get ignore/skipped intentionally or unintentionally while development process due to various reasons.

As part of this document we will try to discuss the following topics:
- [Why we need to make app accessible?](#Why-we-need-to-make-app-accessible?)
- [Different types of accessibility in iOS](#Different-types-of-accessibilities-in-iOS)
- [Voice over Accessibility](#Voice-over-accessibility)
- [Guidelines for voice over attributes](#Guidelines-for-voice-over-attribute)
- [How to test accessibility?](#How-to-test-accessibility?)
- [Example of good and bad accessibility](#Example-of-good-and-bad-accessibility)

## <a name="Why-we-need-to-make-app-accessible?"></a>Why we need to make app accessible?

Accessibility is the topic which we often ignore intentionally or unintentionally while development process. The reasons behind it are several. Some examples are:
* User base using accessibility tools is not big.
* Most of the time we are not using accessibility tools that leads to unawareness.
* Assumption that it slow down the development process
* It does not add the UX design.
* etc ....

**FACT**: Over 1 billion people are estimated to live with some form of physical disabilities. This corresponds to about 15% of the world's population. Along with this more than 100,000 blind and visually impaired individuals could currently own an Apple iPhone - and the number continues to grow, due to aging populations as well as an increase in chronic health conditions.

Business success often depends on the ability to predict future trends and embrace them long before they become mainstream. In this context, we might argue that a seamless mobile experience – and this includes mobile accessibility - is the next important thing in our tech-driven world.

Below is the list of the most important benefits that come from prioritizing mobile accessibility:
* **Extend your market reach** - When you have an accessible mobile solution, you automatically increase the overall number of people that can visit and use your app.
* **Users with physical disabilities can use your application** - Like visual impaired can use your application with the help of voice over.
* **Build brand value** - Consumers prefer to go with brand that is willing to take stand. Building an accessible mobile solution will also help the brand’s reputation.
* **Follow guidelines and minimise legal risks** - Various governing body bodies create guidelines for accessibility. The development of accessibility features in an app can help your business to avoid claims of discrimination and legal actions.
* **It's the right thing to do**


## <a name="Different-types-of-accessibilities-in-iOS"></a>Different types of accessibility in iOS

There are various types of accessibility settings provided in iPhone in iOS 15 as stated below, however not all of them are used for mobile applications.
<details markdown="1">
<summary>Vision</summary>

* [Voice Over](https://support.apple.com/en-gb/guide/iphone/iph3e2e415f/15.0/ios/15.0)
* [Zoom](https://support.apple.com/en-gb/guide/iphone/iph3e2e367e/15.0/ios/15.0)
* [Display and text size](https://support.apple.com/en-gb/guide/iphone/iph3e2e1fb0/15.0/ios/15.0)
* [Motion](https://support.apple.com/en-gb/guide/iphone/iph3e2e1fb0/15.0/ios/15.0)
* [Spoken content](https://support.apple.com/en-gb/guide/iphone/iph96b214f0/15.0/ios/15.0)
* [Audio description](https://support.apple.com/en-gb/guide/iphone/iph96b214f0/15.0/ios/15.0)

</details>

<details markdown="1">
<summary>Physical and motor</summary>

* [AssistiveTouch](https://support.apple.com/en-gb/guide/iphone/iph96b21954/15.0/ios/15.0)
* [Touch accommodations](https://support.apple.com/en-gb/guide/iphone/iph77bcdd132/15.0/ios/15.0)
* [Back tap](https://support.apple.com/en-gb/guide/iphone/iphaa57e7885/15.0/ios/15.0)
* [Reachability](https://support.apple.com/en-gb/guide/iphone/iph145eba8e9/15.0/ios/15.0)
* [Call audio routing](https://support.apple.com/en-gb/guide/iphone/iph29145acf1/15.0/ios/15.0)
* [Vibration](https://support.apple.com/en-gb/guide/iphone/iphd722c9100/15.0/ios/15.0)
* [Face ID and attention](https://support.apple.com/en-gb/guide/iphone/iph646624222/15.0/ios/15.0)
* [Switch Control](https://support.apple.com/en-gb/guide/iphone/iph400b2f114/15.0/ios/15.0)
* [Voice Control](https://support.apple.com/en-gb/guide/iphone/iph2c21a3c88/15.0/ios/15.0)
* [Side or Home button](https://support.apple.com/en-gb/guide/iphone/iph75f461ff0/15.0/ios/15.0)
* [Apple TV remote](https://support.apple.com/en-gb/guide/iphone/iph2ec3a3aa6/15.0/ios/15.0)
* [Pointer control](https://support.apple.com/en-gb/guide/iphone/iphec6e1e60b/15.0/ios/15.0)
* [Keyboards](https://support.apple.com/en-gb/guide/iphone/ipha7c3927eb/15.0/ios/15.0)
* [AirPods](https://support.apple.com/en-gb/guide/iphone/iph345efe861/15.0/ios/15.0)

</details>

<details markdown="1">
<summary>Hearing</summary>

* [Hearing devices](https://support.apple.com/en-gb/guide/iphone/iph470b1833/15.0/ios/15.0)
* [Live Listen](https://support.apple.com/en-gb/guide/iphone/iph8bf9386f5/15.0/ios/15.0)
* [Sound recognition](https://support.apple.com/en-gb/guide/iphone/iphf2dc33312/15.0/ios/15.0)
* [RTT/TTY](https://support.apple.com/en-gb/guide/iphone/iph3e2e47fe/15.0/ios/15.0)
* [Mono audio, balance, and phone noise cancellation](https://support.apple.com/en-gb/guide/iphone/iph3e2e2cdc/15.0/ios/15.0)
* [LED flash for alerts](https://support.apple.com/en-gb/guide/iphone/iph79ced06b1/15.0/ios/15.0)
* [Headphone accommodations](https://support.apple.com/en-gb/guide/iphone/iphb80ab7516/15.0/ios/15.0)
* [Background sounds](https://support.apple.com/en-gb/guide/iphone/iphb2cfa052c/15.0/ios/15.0)
* [Subtitles and captions](https://support.apple.com/en-gb/guide/iphone/iph3e2e23d1/15.0/ios/15.0)
* [Transcriptions for Intercom messages from HomePod](https://support.apple.com/en-gb/guide/iphone/iphe7cd20ce5/15.0/ios/15.0)

</details>

<details markdown="1">
<summary>General</summary>

* [Guided Access](https://support.apple.com/en-gb/guide/iphone/iph7fad0d10/15.0/ios/15.0)
* [Siri](https://support.apple.com/en-gb/guide/iphone/iphaff1d606/15.0/ios/15.0)
* [Accessibility Shortcut](https://support.apple.com/en-gb/guide/iphone/iph3e2e31a5/15.0/ios/15.0)
* [Per-app settings](https://support.apple.com/en-gb/guide/iphone/iph1f48544ab/15.0/ios/15.0)

</details>

As part of this documentation we will focus specifically on **Voice Over** accessibility.


## <a name="Voice-over-accessibility"></a>Voice over Accessibility

VoiceOver is Apple’s innovative screen-reading technology, which gives users control over their devices without having to see the screen. An accessible user interface element must provide accurate and helpful information about its screen position, name, behaviour, value, and type, which is fetched from the different attributes that describe an accessible user interface element. VoiceOver supplies attribute information to users when they access or interact with a control or view.

Below are the different attributes used in voice over
* **Label** - A short, localized word or phrase that succinctly describes the control or view, but does not identify the element’s type. Examples are “Add” or “Play.”
* **Traits** - A combination of one or more individual traits, each of which describes a single aspect of an element’s state, behavior, or usage. For example, an element that behaves like a keyboard key and that is currently selected can be characterized by the combination of the Keyboard Key and Selected traits.
* **Hint** - A brief, localized phrase that describes the results of an action on an element. Examples are “Adds a title” or “Opens the shopping list.”
* **Frame** - The frame of the element in screen coordinates, which is given by the CGRect structure that specifies an element’s screen location and size.
* **Value** - The current value of an element, when the value is not represented by the label. For example, the label for a slider might be “Speed,” but its current value might be “50%.”


## <a name="Guidelines-for-voice-over-attribute"></a>Guidelines for voice over attributes

When VoiceOver users run your application, they rely on the descriptions VoiceOver speaks to understand what your application does and how to use it. Because these descriptions represent the bulk of the VoiceOver user’s experience with your application it’s essential that they be as accurate and helpful as possible

<details markdown="1">
<summary>Guidelines for Creating Labels</summary>

A good way to determine what a label should convey is to think about what a sighted user infers about your application just by looking at it. You should provide a label that:

* **Very briefly describes the element** - Ideally, the label consists of a single word, such as Add, Play, Delete, Search, Favorites, or Volume. Strive to design your application so that a single word identifies an element and makes its usage obvious in the current context. Sometimes, however, it might be necessary to use a brief phrase to properly identify an element. When this is the case, create a very short phrase, such as “Play music,” “Add name,” or “Add to event.”
* **Does not include the type of the control or view** - The type information is contained in the traits attribute of the element and should never be repeated in the label. For example, if you include the control type in the label of an Add button, VoiceOver users hear “Add button button” every time they access that control. This experience would quickly become annoying and might motivate users to stop using your application.
* **Begins with a capitalized word** - This helps VoiceOver read the label with the appropriate inflection.
* **Does not end with a period** - The label is not a sentence and therefore should not end with a period.
* **Is localized** - Be sure to make your application available to as wide an audience as possible by localizing all strings, including accessibility attribute strings. In general, VoiceOver speaks in the language that the user specifies in International settings.

</details>


<details markdown="1">
<summary>Guidelines for Creating Hints</summary>

If the results of a user’s action on a control or view are not clearly implied by its label, create a hint that:

* **Very briefly describes the results** - Even though few controls and views need hints, strive to make the hints you do need to provide as brief as possible. Doing so decreases the amount of time users must spend listening before they can use the element. That said, however, avoid sacrificing clarity and good grammar for brevity. For example, changing “Adds a city” to “Adds city” does not significantly decrease the length of the hint, but does make it sound awkward and a bit less clear.
* **Begins with a verb and omits the subject** - Be sure to use the third-person singular declarative form of a verb, such as “Plays,” and not the imperative, such as “Play.” You want to avoid using the imperative, because using it can make the hint sound like a command. For example, you don’t want to tell users to “Play the song”; instead, you want to tell users that tapping the element “Plays the song.”
  To help you find the right word, imagine that you’re describing the use of a control to a friend. You might say something like “Tapping this control plays the song.” Often, you can use the second phrase in such a sentence (in this case, “Plays the song”) as a hint.

* **Begins with a capitalized word and ends with a period** - Even though a hint is a phrase, not a sentence, ending the hint with a period helps VoiceOver speak it with the appropriate inflection.
* **Does not include the name of the action or gesture** - A hint does not tell users how to perform the action, it tells users what will happen when that action occurs. Therefore, do not create hints such as “Tap to play the song,” “Tapping purchases the item,” or “Swipe to delete the item.”
  This is especially important because VoiceOver users can use VoiceOver-specific gestures to interact with elements in your application. If you name a different gesture in a hint, it would be very confusing.

* **Does not include the name of the control or view** - The user gets this information from the label attribute, so you should not repeat it in the hint. Therefore, do not create hints such as “Save saves your edits” or “Back returns to the previous screen.”
* **Does not include the type of the control or view** - The user already knows whether, for example, the control or view behaves like a button or a search field, because this information is available in the element’s traits attribute. Therefore, do not create hints such as “Button that adds a name” or “Slider that controls the scale.”
* **Is localized** - As with accessibility labels, hints should be available in the user’s preferred language.

</details>


<details markdown="1">
<summary>Identifying Appropriate Traits</summary>

The traits attribute contains one or more individual traits that, taken together, describe the behavior of an accessible user interface element. Below traits can be used:

* **none** - The accessibility element has no traits.
* **button** - The accessibility element behaves like a button.
* **link** - The accessibility element behaves like a link.
* **image** - The accessibility element behaves like an image.
* **searchField** - The accessibility element behaves like a search field.
* **keyboardKey** - The accessibility element behaves like a keyboard key.
* **staticText** - The accessibility element behaves like static text that can't change.
* **header** - The accessibility element is a header that divides content into sections, such as the title of a navigation bar.
* **tabBar** - The accessibility element behaves like a tab bar.
* **summaryElement** - The accessibility element provides summary information when the app starts.
* **selected** - The accessibility element is currently in a selected state.
* **notEnabled** - The accessibility element isn't in an enabled state and doesn't respond to user interaction.
* **adjustable** - The accessibility element allows continuous adjustment through a range of values.
* **allowDirectInteraction** - The accessibility element allows direct touch interaction for VoiceOver users.
* **updatesFrequently** - The accessibility element frequently updates its label or value.
* **causePageTurn** - The accessibility element causes an automatic page turn when VoiceOver finishes reading the text within it.
* **playSound** - The accessibility element plays its own sound when the user activates it.
* **startsMediaSession** - The accessibility element starts a media session when the user activates it.

</details>


## <a name="How-to-test-accessibility?"></a>How to test accessibility?

Accessibility testing can be performed on real device as well as on simulator (using Accessibility Inspector).

### Accessibility testing using Accessibility Inspector
Accessibility inspector is an Xcode tool that is provided by apple in order to test accessibility. It can be launched by choosing Xcode > Open Developer tools > Accessibility inspector in Menu bar or Dock. The Accessibility Inspector presents a utility window that displays the information properties (and values), action methods, and position in the accessibility hierarchy of the object currently on the simulator screen.
You can test the accessibility of elements on screen of simulator using various options in accessibility inspector:

* **Tap on elements on simulator.**
1. Open simulator and launch the app.
2. Select the target simulator on top left corner of accessibility inspector.
4. Select (turns blue when selected) "Target an element." button.
5. Tap on the button for which you want to check the accessibility.
6. Check all the accessibility attributes of the targeted element.

<details markdown="1">
<summary>Target an element example video</summary>

{% include video.html id="accessibility_inspector_Target_an_element.mp4" %}

</details>

* **Play autonavigation to check accessibility of elements on screen.**
1. Open simulator and launch the app.
2. Select the target simulator on top left corner of accessibility inspector.
3. Open the screen in app on which you want to check accessibility.
4. Tap on Speak the element button and click on Start autonavigation button.
5. You can also tap on Previous (<) and forward button (>) to navigate.

<details markdown="1">
<summary>AutoNavigation example video</summary>

{% include video.html id="accessibility_inspector_autonatigation.mp4" %}

</details>

* **Audit an screen** - You can also use Accessibility inspector audit feature to check the accessibility automatically.
1. Open simulator and launch the app.
2. Select the target simulator on top left corner of accessibility inspector.
3. Tap on "Audit" button on top right of accessibility inspector.
4. Tap on "Run Audit" button and wait for audit to be completed.
5. You can also select from options (top right) what all you want to check in audit.

<details markdown="1">
<summary>Auditing example video</summary>

{% include video.html id="accessibility_inspector_auditing.mp4" %}

</details>

* **Other Settings** - You can also test more in accessibility like Dynamic type, Button shapes etc in accessibility inspector.
1. Open simulator and launch the app.
2. Select the target simulator on top left corner of accessibility inspector.
3. Go to Settings on top right corner.
4. Use the scale under dynamic type to test "Zoom".

<details markdown="1">
<summary>Zoom testing example video</summary>

{% include video.html id="accessibility_inspector_font_size.mp4" %}

</details>


### Accessibility testing on real device.
It’s a good idea to test your app on real device using VoiceOver, zoom etc because you can experience the app in the same way that the users will experience it. Using VoiceOver or zoom to run your app can expose problem areas—for example, confusing labels, unhelpful hints, and unreachable elements etc that make your app less accessible

* **Voice Over** - VoiceOver is an iOS Accessibility feature that reads screen descriptions aloud so you can use an iPhone without being able to see the screen.
1. Go to Setting > General > Accessibility > Voice Over.
2. Turn On voice over to use it
3. You can also triple click Home button OR Power button to enable voice over.
4. Tap on element on screen to play voice over for that element.

<details markdown="1">
<summary>Voice over settings image</summary>

   ![Voice over settings]({{ site.baseurl }}/assets/images/voice_over.PNG)

</details>


* **Zoom** - You can zoom in or out on specific items and you can use Zoom together with VoiceOver.
1. Open Settings on your iPhone or iPad.
2. Tap Accessibility.
3. Tap Zoom under the Vision section
4. Tap the switch to turn on Zoom.
5. Tap and drag the slider under Maximum Zoom Level. Left decreases the maximum zoom level, right increases it.

<details markdown="1">
<summary>Zoom settings image</summary>

![Zoom settings]({{ site.baseurl }}/assets/images/zoom.PNG)

</details>


## <a name="Example-of-good-and-bad-accessibility"></a>Example of good and bad accessibility

<details markdown="1">
<summary>Poor Accessibility image</summary>

![Poor Accessibility]({{ site.baseurl }}/assets/images/poor_accessibility.png)

</details>

<details markdown="1">
<summary>Good Accessibility image</summary>

![Good Accessibility]({{ site.baseurl }}/assets/images/good_accessibility.png)

</details>

In the screenshot shown above, you can clearly see difference between poor and good accessibility. In good accessibility example:
* The label of button clearly and shortly states what is the button is for.
* Trait of element is correctly specified.
* Identifier is there to make it testable.
* Hint of element is present to shortly specify what exactly does the element do.
* Meaningful user input is label is available for voice control.

