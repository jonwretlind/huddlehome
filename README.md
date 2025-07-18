# HuddleHome App Specifications

## Family Scheduling and Task App

Create a React Native application for Android that will do the following:

1. Allow administrators to create and assign tasks to family members  
2. Allow administrators to create new events for family member participation  
3. Allow family members to check off tasks and schedule family events  
4. Allow all users to manage their own tasks and schedules

## Purpose

1. The app will help bring family members together by gamifying tasks, chores and events in a fun, interactive and family-friendly way.  
2. The app will create a positive reward system for participation in the daily activities of the family and reinforce positive behaviors  
3. Help reinforce the family’s personal values through a system of rewards, based on personal interests  
4. Suggest new activities that will help the family bond and reinforce shared values

## Features

1. App will create a gamification system with points earned for completing tasks and participating in events  
2. App will allow searching for new events in their community based on personal interests  
3. App will allow users to accumulate points for participation and completion of tasks  
4. Administrators can:  
   1. Create new tasks  
   2. Assign tasks to family members  
   3. Assign point values to tasks and events  
   4. Create unassigned tasks that can be completed by any family member  
   5. Create events  
   6. Delete tasks and events  
   7. Create group challenges for tasks and events  
   8. Grant points to family members  
   9. Create goals based on personal interests and personal values  
5. All users can:  
   1. Complete tasks  
   2. Accept new tasks that are unassigned  
   3. Attend events  
   4. Accumulate points  
   5. Participate in group challenges  
   6. Share points and allow for reaching personal goals in a positive way

## Technical Considerations

1. Website URL: HuddleHome.casa  
2. Use React Native for app  
3. Use most recent Google Material Design Standards for app and icons  
4. For website front-end, employ Tailwind libraries for style and UX  
5. Use a modern, playful theme employing a glassmorphic sleek style for UI elements  
6. For Backend, API and website is to be hosted on AWS EC2 instance  
7. Download and employ up-to-date Javascript/Typescript libraries and React components as needed for app functionality

### Frontend Security

| Security Measure | Description |
| ----- | ----- |
| Use HTTPS everywhere | Prevents basic eavesdropping and man-in-the-middle attacks |
| Input validation and sanitization | Prevents XSS attacks by validating all user inputs |
| Don't store sensitive data in the browser | No secrets in localStorage or client-side code |
| CSRF protection | Implement anti-CSRF tokens for forms and state-changing requests |
| Never expose API keys in frontend | API credentials should always remain server-side |

### Backend Security

| Security Measure | Description |
| ----- | ----- |
| Authentication fundamentals | Use established libraries, proper password storage (hashing+salting) |
| Authorization checks | Always verify permissions before performing actions |
| API endpoint protection | Implement proper authentication for every API endpoint |
| SQL injection prevention | Use parameterized queries or ORMs, never raw SQL with user input |
| Basic security headers | Implement X-Frame-Options, X-Content-Type-Options, and HSTS |
| DDoS protection | Use a CDN or cloud service with built-in DDoS mitigation capabilities |

### Practical Security Habits

| Security Measure | Description |
| ----- | ----- |
| Keep dependencies updated | Most vulnerabilities come from outdated libraries |
| Proper error handling | Don't expose sensitive details in error messages |
| Secure cookies | Set HttpOnly, Secure and SameSite attributes |
| File upload security | Validate file types, sizes, and scan for malicious content |
| Rate limiting | Implement on all API endpoints, especially authentication-related ones |

A special thanks to [Ted](https://x.com/tnm/status/1903507404840747198) for the [inspiration](https://gist.github.com/tnm/713276279392a2edb4ff7ff5f1efe43c).

## UI Considerations

1. The app will be a native mobile application for the Android or iOS devices  
2. The codebase will be scalable and allow for easy maintenance  
3. The system will be expandable with new features  
4. The core of the system will be gamified in allowing points to be exchanged for rewards specified by administrative users  
5. The app will be downloadable as a purchase through Google Play or the Apple Store  
6. Once purchased, each family member will have access to the application based on role  
7. The app will have a modern, family-oriented and fun easy-to-use interface with a playful feel.  
8. Ease of use will be paramount consideration

## Design Considerations

The design style of HuddleHome app and websites should be friendly, engaging and fun in tone with flat-style cartoon graphics and colorful, sporty look and feel.

### Color Palette

/\* CSS HEX \*/  
\--robin-egg-blue: \#25ced1ff;  
\--white: \#ffffffff;  
\--champagne-pink: \#fceadeff;  
\--coral: \#ff8a5bff;  
\--bright-pink-crayola: \#ea526fff;

/\* CSS HSL \*/  
\--robin-egg-blue: hsla(181, 70%, 48%, 1);  
\--white: hsla(0, 0%, 100%, 1);  
\--champagne-pink: hsla(24, 83%, 93%, 1);  
\--coral: hsla(17, 100%, 68%, 1);  
\--bright-pink-crayola: hsla(349, 78%, 62%, 1);

/\* SCSS HEX \*/  
$robin-egg-blue: \#25ced1ff;  
$white: \#ffffffff;  
$champagne-pink: \#fceadeff;  
$coral: \#ff8a5bff;  
$bright-pink-crayola: \#ea526fff;

/\* SCSS HSL \*/  
$robin-egg-blue: hsla(181, 70%, 48%, 1);  
$white: hsla(0, 0%, 100%, 1);  
$champagne-pink: hsla(24, 83%, 93%, 1);  
$coral: hsla(17, 100%, 68%, 1);  
$bright-pink-crayola: hsla(349, 78%, 62%, 1);

/\* SCSS RGB \*/  
$robin-egg-blue: rgba(37, 206, 209, 1);  
$white: rgba(255, 255, 255, 1);  
$champagne-pink: rgba(252, 234, 222, 1);  
$coral: rgba(255, 138, 91, 1);  
$bright-pink-crayola: rgba(234, 82, 111, 1);

/\* SCSS Gradient \*/  
$gradient-top: linear-gradient(0deg, \#25ced1ff, \#ffffffff, \#fceadeff, \#ff8a5bff, \#ea526fff);  
$gradient-right: linear-gradient(90deg, \#25ced1ff, \#ffffffff, \#fceadeff, \#ff8a5bff, \#ea526fff);  
$gradient-bottom: linear-gradient(180deg, \#25ced1ff, \#ffffffff, \#fceadeff, \#ff8a5bff, \#ea526fff);  
$gradient-left: linear-gradient(270deg, \#25ced1ff, \#ffffffff, \#fceadeff, \#ff8a5bff, \#ea526fff);  
$gradient-top-right: linear-gradient(45deg, \#25ced1ff, \#ffffffff, \#fceadeff, \#ff8a5bff, \#ea526fff);  
$gradient-bottom-right: linear-gradient(135deg, \#25ced1ff, \#ffffffff, \#fceadeff, \#ff8a5bff, \#ea526fff);  
$gradient-top-left: linear-gradient(225deg, \#25ced1ff, \#ffffffff, \#fceadeff, \#ff8a5bff, \#ea526fff);  
$gradient-bottom-left: linear-gradient(315deg, \#25ced1ff, \#ffffffff, \#fceadeff, \#ff8a5bff, \#ea526fff);  
$gradient-radial: radial-gradient(\#25ced1ff, \#ffffffff, \#fceadeff, \#ff8a5bff, \#ea526fff);

### Fonts

For emphasis and headings:  
.playpen-sans-\<uniquifier\> {  
  font-family: "Playpen Sans", cursive;  
  font-optical-sizing: auto;  
  font-weight: \<weight\>;  
  font-style: normal;  
}

For smaller normal text:  
// \<weight\>: Use a value from 100 to 900  
// \<uniquifier\>: Use a unique and descriptive class name

.noto-sans-\<uniquifier\> {  
  font-family: "Noto Sans", sans-serif;  
  font-optical-sizing: auto;  
  font-weight: \<weight\>;  
  font-style: normal;  
  font-variation-settings:  
    "wdth" 100;  
}

