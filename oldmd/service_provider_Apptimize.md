
## Apptimize

Apptimize allows iOS and Android teams to make real-time updates to the native app experience and data-driven product decisions. Teams can A/B test user flows, control feature rollouts, make instant UI changes, and more.

### Supported Features

A/B Testing

### Prerequisites

In order to enable mParticle’s integration with Apptimize, you will need your App Key which can be found on your Apptimize [settings](https://apptimize.com/admin/settings/apps) page.

### Apptimize Kit Integration

mParticle's Apptimize integration requires that you add the Apptimize kit to your iOS or Android app, and the mParticle SDK will initialize and automatically map mParticle method calls directly onto Apptimize method calls. This approach means that *every feature* of the Apptimize SDKs are supported, as if the app had integrated Apptimize directly. The source code for each kit is available if you would like to learn exactly how the method mapping occurs:

- [iOS](https://github.com/mparticle-integrations/mparticle-apple-integration-apptimize)
- [Android](https://github.com/mparticle-integrations/mparticle-android-integration-apptimize)

~~~objc
//Sample Podfile
target '<Your Target>' do
    pod 'mParticle-Apptimize', '~> 6'
end
~~~

~~~java
//Sample build.gradle
dependencies {
    compile ('com.mparticle:android-apptimize-kit:4.+')
}
~~~   

Add the Apptimize Kit to your iOS or Android app. See the Cocoapods and Gradle examples to the right, and reference the [Apple SDK](https://github.com/mParticle/mparticle-apple-sdk) and [Android SDK](https://github.com/mParticle/mparticle-android-sdk) GitHub pages to read more about kits.

### Apptimize mParticle Configuration

Create a Apptimize output configuration:

1.  Select **Directory**, and click the Apptimize tile
2.  Click **Add Apptimize to Setup**
3.  Select the **Output Event** Integration Type and click **Add to Setup**
4.  Select the **Apptimize** output configuration group to configure an output event configuration
5.  Enter a Configuration Name and your Apptimize configuration settings and click **Save**

Connect inputs to the Apptimize output configuration

1.  Select **Connections**
2.  Select the Input for the connection definition
3.  Click **Connect Output**
4.  Select the **Apptimize** configuration
5.  Enter your connection configuration settings
6. Toggle the Status to **Sending**
7. Click **Save**