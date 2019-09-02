---
title: 'Updated: How to Customize YouCanBook.me for Appointment Slots'
date: 2019-01-01
permalink: /2019/01/01/you-can-book-me/
categories:
  - advising
  - technology
  - tutorial
---
One of the most popular posts that I originally wrote in December 2012 was the tutorial below on customizing the YouCanBook.me calendar service to display appointment slots -- such as "office hours" -- using your Google Calendar. Until 2018, this option was free for educators who received a non-profit account, but it is **NO LONGER FREE**. But the notes below may be helpful for people (like me) who now pay to use this service, since as of early 2019 I still have not found a good replacement that allows me to manage office hour slots from within my Google Calendar application.

<em>Updated on March 23, 2016:</em>&nbsp;Here's the new link to request an education account, which no longer appears to be automatic for users who log in with an .edu email address:&nbsp;<a href="https://youcanbook.me/feature/community/">https://youcanbook.me/feature/community/</a>

<em>Updated on February 26, 2015: </em>The friendly folks at YouCanBook.Me tell me that the "On Duty" feature (which displays my office hours, as described below) now requires a paid premium-level subscription OR a free non-profit account. <del>Users who log in with an .edu email address automatically qualify for a free non-profit account</del>, or you can request one by visiting their <a href="https://gb.youcanbook.me/nonprofit.jsp">Non-Profit help page</a>. Also, for more up-to--date instructions, see also YouCanBook.Me's own <a href="https://ga.youcanbook.me/feature/onduty">tutorial on using the "On Duty"</a> (aka "office hours") feature.

<em>Updated from original Dec 2012 post:</em>
In case your end-of-semester meeting calendar was so busy that you didn't notice, Google recently <a title="announcement" href="http://googleblog.blogspot.com/2012/12/winter-cleaning.html" >announced that it will shut down the ability to create new Google Calendar Appointment slots</a>&nbsp;on&nbsp;January 4, 2013. Like me, many faculty may have first learned about online scheduling tools that enable students and colleagues to automatically book appointments from Heather Whitney's <a title="ProfHacker" href="http://chronicle.com/blogs/profhacker/scheduling-101-appointment-slots-in-google-calendar/34575" ><em>ProfHacker</em> post (July 2011)</a>&nbsp;and <a title="ProfHacker" href="http://chronicle.com/blogs/profhacker/follow-up-appointments-slots-in-google-calendar/37209" >follow ups in (November 2011)</a>&nbsp;and&nbsp;<a href="http://chronicle.com/blogs/profhacker/google-calendar-cancels-appointment-slots-implications-for-scheduling-office-hours/45067" >December 2012</a>).&nbsp;Publicly displaying selected blocks of time from my Google Calendar made life much easier for me, and those trying to connect with me, while avoiding those annoying "When are you free?" or "Monday doesn't work, how about Tuesday?" email exchanges. Many students told me they actually <em>liked</em>&nbsp;the Appointment slots feature as an automated way of making time for in-depth conversation, rather than catching me for a haphazard hallway chat. But what the Google gave, the Google hath taken away, with <a title="GoogleProductForums" href="https://productforums.google.com/forum/?fromgroups=#!topic/calendar/chG8bTXFbbE" >great disappointment to many disciples</a>. Another popular online appointment scheduler, <a title="tungle" href="http://www.tungle.me/blog.html" >Tungle, also shut down</a> in December 2012.

Looking around for alternative tools helped clarify which features were most valuable to me. Organizing group meetings is great with <a title="Doodle MeetMe" href="http://www.doodle.com/about/meetMe.html" >Doodle, but its MeetMe personal scheduler</a> &nbsp;did not allow for automatic appointment booking, meaning that I'd need to confirm each individual. Another service, <a title="TouchBaseIt" href="http://www.touchbase.it/" >TouchBase.it</a>, integrates a personal scheduling assistant into Google Mail (great for many students), but I could not customize the default 1-hour appointment blocks into smaller units (20-minute blocks seem best for most of my student meetings.) A more sophisticated tool, <a title="ScheduleOnce" href="http://www.scheduleonce.com/" >ScheduleOnce.com</a>, offered the date- and time-specific appointment flexibility I desired, and tempted me with its free 14-day trial offer, but my real cost for automatic booking would be $9 per month. Maybe one of these tools works for you (or your budget), but none satisfied me.

Then I looked back at <a title="YouCanBookMe" href="http://youcanbook.me/" >YouCanBook.Me</a>, a free service that I had initially dismissed as too inflexible, and discovered that it offered all of the features I desired, after I deciphered an obscure phrase in the user interface. Here's instructions and screenshots on how I've customized the settings (with one suggested revision for the developer).

1) Create a YouCanBook.Me account (using your Google login) and walk through the setup pages (accepting defaults, for now) to link to your Google Calendar.

![](/images/2012/YouCanBookMeSetup.png)

2) Launch the Settings Editor, and under the Basic tab, design your header page.

![](/images/2012/YouCanBookMeBasicScreen.png)

3) Under the Times tab, click ALL days of the week and hours when you might PLAUSIBLY be available to meet (such as Mon-Fri, 8am-5pm, which we'll modify soon). On the right side, designate a booking time (mine is 20 minutes). Now for the hidden step: pretend that the field labeled "on duty events" says something more useful, such as "Customize my times to match available Google Calendar events with this phrase." Insert your exact phrase into the text box (mine is "office hours").

![](/images/2012/YouCanBookMeTimesScreen.png)

4) In your Google Calendar, create an event that matches your phrase ("office hours"). Near the bottom, change its default display from show me as "busy" to "available."

![](/images/2012/YCBMGoogleCalendarEvent.jpg)

5) In the YouCanBookMe dashboard, publish your booking page online, and share the link and/or embed on your website. Appointment-seekers will see only the available slots that you have designated in your settings.

![](/images/2012/YouCanBookMeUserView.png)

6) When appointment-seekers select a slot and enter their email address, they receive a confirmation message in their inbox. Fortunately, YouCanBook.Me does NOT require other users to have a Google Calendar in order to book a slot with you (which is a clear advantage over the old system), but a great feature is that their confirmation email includes a handy link to add the appointment to their Google Calendar if they happen to have one.

![](/images/2012/YouCanBookMeBookingScreen.png)

7) Here's the magic: when users book appointments during my office hours slots, it automatically appears in my Google Calendar.&nbsp;Furthermore, if I manually schedule an appointment for another student during my office hours, it automatically removes that slot from the display of available times (which is a huge improvement over the old Google Calendar Appointment slots).

![](/images/2012/YouCanBookMeGCalBookedView.png)

8) iOS Cal users: watch out for accidental overrides. If you create an "all-day" event on your calendar and the default setting is "busy," it will accidentally block out any appointments that you have available to fill. This issue stumped me until I figured out the underlying problem. When I create all-day events in Google Calendar, the default is "available," so that worked just fine. But when I create all-day events in my iPhone's Calendar application (which is linked to my Google Calendar data), the default is "busy," which overrides all appointment slot availability that day for my students. Oops. Gotta remember to switch those all-day iOS Cal entries from "busy" to "free."

9) Back inside your YouCanBookMe dashboard, you can manage information fields to be collected in the automatic booking form (I added a spot for appointment-seekers to add the topic they'd like to discuss), along with more advanced display settings. For example, to move the calendar grid from the center of the web page to the left margin, under the "appearance" tab, I inserted this bit of CSS code to override the default.

![](/images/2012/YouCanBookMeAppearanceCSS.png)

I discovered these steps after reading the&nbsp;<a title="YCBM help tool" href="http://feedbackfrenzy.com/service/item.jsp?instance=ycbm&amp;item=uvHaDGFbPdfrf2au2QP4" >YouCanBookMe's online help tool on non-standard start &amp; end times (the "stencil" feature)</a>. If the company makes the interface and documentation clearer to newcomers, their tool is likely to be adopted by many former Google Calendar Appointment slots users. I hope that YCBM enjoys a longer life span on the web.
