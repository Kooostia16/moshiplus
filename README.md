![MoshidonLogo](mastodon/src/main/res/mipmap-xhdpi/ic_launcher_round.png)

# Moshiplus 

> A fork of [moshidon](https://github.com/LucasGGamerM/moshidon)

--- 

## Key features

### **The ability to add other server's local timeline to your timelines**

It can be accessed in the "Edit timelines" menu, where you can add a new "Community" to see other server's local posts!

### **View remote profiles**

You can now see all of a profile follows and followers, by directly loading them from the profile's home instance. In case of a failed lookup, the app will automatically fall back to the older method.

### **Translate posts easily**

Allows you to easily translate posts in another language with a translate button! Your instance must support translation, otherwise it will not work.

### **Show posts filtered with a warning**

Allows you to have filtered posts collapsed with a warning! As shown in the screenshots:

Before             |  After
:-------------------------:|:-------------------------:
![Screenshot_20230205-100200edited](https://user-images.githubusercontent.com/71328265/216820539-20802dc5-e433-4511-b2d9-291d810e4ef2.png) | ![Screenshot_20230205-100203edited](https://user-images.githubusercontent.com/71328265/216820544-231b2966-f38f-4ec6-b555-d39c62433839.png)


### **Color themes**

Allows you to change theme within the app. Supports Material You, purple, pink, green, blue, red, orange, yellow and Nord!

### **Unlisted posting**

**Allows you to post publicly without having your post show up in trends, hashtags or public timelines (i.e., in the tabs “Local”, “Community” and “Posts”).**

When posting with Unlisted visibility, your posts will still be publicly accessible in your profile. They will also be shown in people’s Home timelines, but only if they follow you or someone they follow reposted/replied to your post.
  
The Mastodon documentation has some more information about [Unlisted posting](https://docs.joinmastodon.org/user/posting/#unlisted) and [Public timelines](https://docs.joinmastodon.org/user/network/#timelines).

### **Federated timeline**

**This allows you to chronologically see all Public posts from people on all other Fediverse neighborhoods your home instance is connected to.**

Despite being one of the main features of federated social media, the Federated timeline wasn’t included in the official Mastodon app – supposedly, because this conflicts with Google’s safety requirements for apps on the Play Store.
  
That’s one of the reasons why choosing a small, **well-moderated instance is important**. Instance admins and moderators should always make sure to ban abusive users and stop federating with instances who platform them. On well-moderated instances, the Federated timeline can be a welcoming place to meet new people!

### **Image description viewer**

**Allows you to quickly check whether an image or video has an alternative text attached to it.**

This is important to **ensure the content you’re sharing is as accessible as possible** to people who can’t see the images and rely on software to read back the provided content descriptions. Thankfully, it’s quite common for people on the Fediverse to provide such alt texts, and hopefully things stay this way!

### **Reminder to add alt text to attached media**

By default, Moshiplus will show a warning to add alt text if your post has any attachments without any alt text. This is for better accessibility, and it can easily be bypassed and disabled in settings.

### **Pinning posts**

**This lets you can highlight important posts on your profile. A dedicated “Pinned” tab in people’s profiles shows all the posts they pinned.**

On the Fediverse, it’s quite common for people to pin posts they want others to read before following them. You can pin/unpin posts yourself by clicking the `⋯` button in the top right corner of your posts.

### **Bookmarks**

**They allow for quickly saving posts and viewing them through the Bookmarks button on the top right of your profile.**

To bookmark a post, press the button between the Favorite and Share buttons on the bottom of the post. Bookmarks are saved privately, so the post authors won’t know you saved their post – the list of bookmarked posts is only visible to you.

## Installation

## Release variants

### Stable variant

All stable version downloads can be found on the Releases page.

### Nightly variant

Unstable variant with an integrated updater. It's for development and testing purposes. If you find any bugs with it, please file a bug report at our issues page.

---


## Detailed changes

### Features

* Adding the ability to view other server's local timelines
* Adding the ability to load followers and following from remote instance
* Adding the ability to have filtered posts show with a warning
* Add “Unlisted” as a post visibility option
* Adding a useful private profile note box
* Auto hiding the compose button on scroll
* Adding the ability to remind yourself to add alt text to images
* An indicator for if an image has alt text or not
* Adding the ability to have drafts
* Also adding the ability to view announcements from your instance
* Adding the ability to post for local timeline only (Only on instances that support it!)
* Add image description button and viewer
* Implement pinning posts and displaying pinned posts
* Implement deleting and re-drafting
* Implement a bookmark button and list
* Add “Check for update” button in addition to integrated update checker
* Add “Mark media as sensitive” option
* Add settings to hide replies and reposts from the timeline
* Follow and unfollow hashtags
* Notification bell for posts
* Viewing lists and adding/removing users from lists
* List favorited posts
* Accept/reject follow requests
* Display content warning title above text
* Add notifications tab for posts
* Show visibility of original post when replying
* Clickable reply/boost line above posts
* Clickable reply line while replying to open original post


### Behavior

* Allow for confirmation before reblogging
* Adding a bottom option for the publish button, allowing for easier use on larger screens!
* Make back button return to the home tab before exiting the app
* Always preserve content warnings when replying
* Display full image when adding image description
* Set spoiler height independently to content height
* Option to hide interaction numbers
* Option to always reveal content warnings
* Option to disable scrolling title bars


### Visual

* Custom extended footer redesign
* Improvements to the true black mode
* Profile header tweaks


## Building

As this app is using Java 17 features, you need JDK 17 or newer to build it. Other than that, everything is pretty standard. You can either import the project into Android Studio and build it from there, or run the following command in the project directory:

```
./gradlew assembleRelease
```

## License

This project is released under the [GPL-3 License](./LICENSE).

## Links

[F.A.Q](FAQ.md)

---
