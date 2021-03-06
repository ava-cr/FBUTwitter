# Project 3 - *AvasTwitter*

**AvasTwitter** is a basic twitter app to read and compose tweets the [Twitter API](https://apps.twitter.com/).

Time spent: **24** hours spent in total

## User Stories

The following **required** functionality is completed:

- [X] User sees app icon in home screen and styled launch screen
- [X] User can sign in using OAuth login flow
- [X] User can Logout
- [X] User can view last 20 tweets from their home timeline
- [X] In the home timeline, user can view tweet with the user profile picture, username, tweet text, and timestamp.
- [X] User can pull to refresh.
- [X] User can tap the retweet and favorite buttons in a tweet cell to retweet and/or favorite a tweet.
- [X] User can compose a new tweet by tapping on a compose button.
- [X] Using AutoLayout, the Tweet cell should adjust its layout for iPhone 11, Pro and SE device sizes as well as accommodate device rotation.
- [X] User should display the relative timestamp for each tweet "8m", "7h"
- [X] Tweet Details Page: User can tap on a tweet to view it, with controls to retweet and favorite.

The following **optional** features are implemented:

- [X] User can view their profile in a *profile tab*
  - Contains the user header view: picture and tagline
  - Contains a section with the users basic stats: # tweets, # following, # followers
  - [X] Profile view should include that user's timeline
- [X] User should be able to unretweet and unfavorite and should decrement the retweet and favorite count. Refer to [[this guide|unretweeting]] for help on implementing unretweeting.
- [X] Links in tweets are clickable.
- [X] User can tap the profile image in any tweet to see another user's profile
  - Contains the user header view: picture and tagline
  - Contains a section with the users basic stats: # tweets, # following, # followers
- [X] User can load more tweets once they reach the bottom of the feed using infinite loading similar to the actual Twitter client.
- [X] When composing, you should have a countdown for the number of characters remaining for the tweet (out of 280) (**1 point**)
- [X] After creating a new tweet, a user should be able to view it in the timeline immediately without refetching the timeline from the network.
- [X] User can reply to any tweet, and replies should be prefixed with the username and the reply_id should be set when posting the tweet (**2 points**)
- [ ] User sees embedded images in tweet if available
- [X] User can switch between timeline, mentions, or profile view through a tab bar (**3 points**)
- [ ] Profile Page: pulling down the profile page should blur and resize the header image. (**4 points**)


The following **additional** features are implemented:

- [X] Tweets from users with protected accounts (tweets that you can't retweet) have greyed out and disabled retweet buttons.

Please list two areas of the assignment you'd like to **discuss further with your peers** during the next class (examples include better ways to implement something, how to extend your app in certain ways, etc):

1. Multiple custom cells in table views.
2. Dynamically changing table view cells/their content. For ex. with adding images to table view cells when you don't know whether or not there will be images or how many there will be.

## Video Walkthrough

Here's a walkthrough of implemented user stories:

1. App icon, log in/log out (on iPhone 8)

<img src='https://github.com/ava-cr/FBUTwitter/blob/main/gifs/twitter1.gif' title='Video Walkthrough 1' width='' alt='Video Walkthrough' />

2. Home timeline with tweets (profile pic, tweet details, timestamps, etc), pull-to-refresh, infinite scrolling (iPhone 11)

<img src='https://github.com/ava-cr/FBUTwitter/blob/main/gifs/twitter2.gif' title='Video Walkthrough 2' width='' alt='Video Walkthrough' />

3. Like/unlike, retweet/unretweet, reply to a tweet/compose a tweet with character limit (on iPhone 11)

<img src='https://github.com/ava-cr/FBUTwitter/blob/main/gifs/twitter3.gif' title='Video Walkthrough 3' width='' alt='Video Walkthrough' />

4.  Tab bar to see timeline/mentions/profile view, profile view has user's timeline, auto-layout in different device sizes/rotation (on iPhone 11)

<img src='https://github.com/ava-cr/FBUTwitter/blob/main/gifs/twitter4.gif' title='Video Walkthrough 4' width='' alt='Video Walkthrough' />

5.  Click on tweet to view a tweet details page, click on a user's profile picture to view their profile page, clickable links (on iPhone 11).

<img src='https://github.com/ava-cr/FBUTwitter/blob/main/gifs/twitter5.gif' title='Video Walkthrough 5' width='' alt='Video Walkthrough' />

GIFs created with [Kap](https://getkap.co/).

## Notes

Describe any challenges encountered while building the app.

I wanted to add the number of replies a tweet had to my tweet cell (along with # of favorites and # of retweets) but reply_count "is only available with the Premium and Enterprise tier products" and so I struggled with why it was returning 0 for a minute. Also, I didn't know that you could have multiple different custom table view cells within a table view so I struggled with how to implement the profile tab before finding this out from my manager (shout-out Kyle).

## Credits

List an 3rd party libraries, icons, graphics, or other assets you used in your app.

- [AFNetworking](https://github.com/AFNetworking/AFNetworking) - networking task library
- 
    [DateTools](https://github.com/MatthewYork/DateTools#time-ago) - library to streamline date and time handling in iOS.

## License

    Copyright [2021] [Ava Crnkovic-Rubsamen]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
