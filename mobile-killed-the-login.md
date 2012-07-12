Logins are Dead, and Mobile Killed Them
=======================================

Logging in with a username and password is dead; Mobile killed it.

Why is it dead? Because you and your phone are _one thing_; a single organism. You get [extremely nervous](http://en.wikipedia.org/wiki/Nomophobia) when you're parted from it. It is your _precious_; once you get past the lock screen, you are intimately connected to it. And [83% of young people](http://www.onlineschools.org/visual-academy/always-connected/) go to bed with their phone. Some older ones too. This is _not_ a shared device or even that thing you leave lying around on your desk unattended.

And logins are dead because typing a username and password on mobile is both a _horrible_ and _unsafe_ experience. Horrible because smartphones are not good devices for accurate typing and unsafe because people use their phone in public spaces like a bus where someone may be looking over your shoulder.

Story Time
----------

I want to tell you the story of something we built into our mobile apps at <a href="http://www.local.ch">local.ch</a> as part of a product which finally got <a href="http://www.telecompaper.com/news/localch-offers-real-time-mobile-business-alerts">announced today</a>. Doing that will help me make sense of all this, so bear with me...

So <a href="http://www.local.ch">local.ch</a> is a bit like the Swiss Yelp, the official Yellow and White pages for Switzerland. I'm priveliged to be able to lead an [awesome team](https://twitter.com/#!/hfuecks/local-ch-mobile) and we make apps for pretty much [all smartphones](http://info.local.ch/directories/mobile) plus a [mobile website](http://mobile.local.ch) which is [work in progress](http://i.local.ch). Apple recently ranked our iOS app as [the 4th most popular free app in Switzerland](http://www.20min.ch/digital/dossier/apple/story/Die-beliebtesten-iPhone-Apps-aller-Zeiten-28833506). By the way Switzerland is Apple territory with somewhere between 2 and 3 million iOS devices out there, bearing in mind a total population of about 7.8 million. We're proud to boast we've had over 1.7 million downloads, 1.1 million of those being iOS and another ~ 400k being Android.

Now local.ch has a field sales force of around 400 people, and every day they're touring the country visiting our SME customers and helping them to promote their business with our ad products. One of those products is <a href="http://www.telecompaper.com/news/localch-offers-real-time-mobile-business-alerts">Mobile Business Alerts</a>; a kind of "twitter for SMEs" allowing them publish the type of content they might put in a shop window such as "20% off shoes" or "Menu of the Day".

Still with me?

We all hate logins
------------------

local.ch hates them because they cause adminstration costs. Our customers hate them because they're busy, busy people. Busy running their businesses with no time for "What was my password again?". Engineers and product managers hate them because you have to build lots of sucky forms which are never quite are as usuable as they should be and lead to missed deadlines.

So we got rid of them. No username / password login required to access this product. And we chose Facebook / Twitter / OAuth right? Nope. It's a shitty position to be in when you have this large, deaf middle-man between you and your customers. Period.

It's just simple
----------------

In it's essence our approach is very simple; we activate the _device_.

We send you a link by SMS or E-Mail containing a link comprised of an activation code. Tapping on the link results in our app being launched in "activation mode". The app then "phones home" passing back the activation code and some unique identifier for the device. That's it.

We're now able to identify you so we can enable your "super powers" in the form of [functionality](http://mba.local.ch/en/2012/07/12/step-by-step-your-first-offer/) that normal users of our app don't have access to. So long as you keep your phone and remain a local.ch customer, you keep your "super powers".

I've skipped a bunch of technical details here but that describes the essence of the process. [These guys](https://twitter.com/#!/hfuecks/local-ch-mobile) did an awesome job of making it watertight so ask them if you want specifics.

For the end user it's simply "open message, tap link, done! Forever". That's a pain-free experience.

A Graph of Approval
-------------------

One of the inspirations which led to this design was [Bump](https://bu.mp/); the idea that we could pass authorization from person to person much like Bump allows you to pass contact details. Why? Because this is a great match to our typical sales process; pitch product face-to-face, sign contract, activate phone.

In practice, when we train our sales people, we activate their phones with "sales super powers". Then, whenever they _sell_ our product, they become the "kingmaker", activating the customer right from our app, via SMS or E-Mail. We're even happy for the customer to forward the activation message to their own employees. If there's any trouble, such as lost phone or employee leaving, the customer just requests a new activation message, resetting all devices that were previously activated.

Side note: why didn't we use Bump after all? A little too freaky for our sales to work with and project deadlines which made tried and tested tools like E-Mail and SMS very attractive.

What would Steve do?
--------------------

The other spark of inspiration came from Apple.

Have you ever noticed how they insist on a _personal_ E-Mail when you have an Apple Developer account? While it may drive IT departments crazy, Apple disapproves of "group" emails like admins@foo.com. They want a name; a _person_ they know will take responsibility when they need to get in touch. I find it pretty amazing a company of Apple's size works this way and it really got me thinking about the philosophy behind it.

Mobile enables that idea of being _personal_ to take shape in a intimate way, one that's good enough to grant super powers with.

But, but, but...
----------------

As strict security systems go, this obviously has a lot of limitations but for what we're dealing with, we felt it didn't matter. Of course there's a whole bunch of cases I'm happily ignoring, like banking apps, the App Store and pretty much anything with money changing hands.

In our case, were anyone to steal your phone, we're quickly able to undo anything malicious and de-activate the phone stopping them for good. And sure I may end up eating my words but this is about _good enough_ security.

And since the soft launch of our product, back in March 2012, our 400+ customers have generated less than 30 cases for our support helpdesk, so we think it's more than good enough. And our customers love it, allowing them focus on the product we deliver, not the annoying login form that prevents them using it.

Implications
------------

When I look at [what the big guys are doing](https://plus.google.com/105166600541125352541/posts/GZ2ePMeUjLG) I think this might be a a break through; a different way of looking at the problem which takes advantage of what mobile brings us.

Right now I should probably invent a smart name for it (oh AJAX, I'm still bitter) but perhaps it's not such a big thing after all so I won't bother. Excuse me - I'm English.

And without getting _too_ far out there, I think there is some room here to shake up this thing we've been calling the "identity layer".

Questions? @hfuecks