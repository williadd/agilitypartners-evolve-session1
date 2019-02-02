# agilitypartnerers-evolve-session1

## Week 1 - Intro to Rails
- Ruby environment
- Ruby language
- Getting started with unit testing
- Hello World in Rails
- Code quality intro

[Week 1 Slides](content/Rails%20-%20Week%201.pdf)

[Week 1 Supplement](content/Week%201%20Supplementary.pdf) (remember, this was going to be the lecture of class was cancelled)

## Week 1 Assignment - Calculator with Rails
Yes, this is way overkill to use Rails to build a simple calculator. This is not an exercise to see if you can build a calculator, it's intended to make you use some of the controller and view so that you begin to understand where everything goes and the request-response cycle in Rails.

Build a calculator that 
- has the numbers 1-9 as separate buttons
- supports addition and subtraction
- Has the user entering things in the format "1 + 1 =" using buttons

Please do not just use some Javascript to solve the problem in a single page. Though, you may need to use a little Javascript to get some field assignments to work properly.

## Week 2 - Scaffolding and Persistence
- Scaffolding basics
- Routes and REST
- Testing in Rails
- ActiveRecord and Models

[Week 2 Slides](content/Rails%20-%20Week%202.pdf)

## Week 2 Assignment - Company Employee Listing
Looking for an applivation that allows the user to manage the employees for many companies. Want to be able to do the following
- View and manage a list of companies
- View and manage the employees for each of those companies
- see the count of employees for each company
- search for employees matching a portion of a name

Scaffolding will create a lot of this for you, but it won't be pretty, so you may want to add a little style to the generated pages. Don't worry about pagination right now. Active Record does have capabilities to help with that, though. You will need to create your own content for the search page.

## Week 3 - Testing, More about Routes
- testing controllers and models
- mocking
- executing code quality tools with Rake
- Nesting routes and route aliasing
- Cookies and Sessions

[Week 3 Slides](content/Rails%20-%20Week%203.pdf)

## Week 3 Assignment - AgilityPartnersWireless.com
We're going to build a new wireless provider! This project will take 2 weeks and will use all of the things we've learned so far. There is 3 aspects to this
1. site for the provider to manage devices and accounts
1. site for customers to buy devices and manage their accounts
1. device emulators

It's going to be a little complex. The device emulators will be really dumbed down, just a simple page that has some numbers and can place fake calls and send fake text threads.

Here's some functionality needed, at a high level.

AP Wireless customer service
- locate customer accounts by account number, phone number, or by name (e.g. searching for John should bring back John Smith or Elton John)
- see what devices a customer has on their account
- see summary information about device activity
- manage devices available through AP Wireless, including inventory levels

AP Wireless user site
- create a new account or access an existing account (by phone number)
- "purchase" decvices and add them to your account
- see usage for devices on your account
- deactivate a device

Phone emulators
- make phone calls 
  - nobody is receiving the call, but the receiver would be able to see the call log
- send texts
  - nobody receives the text in real time, but the reciever should be able to see the thread
  
As noted above, this is meant to use a lot of the things we've learned about. You'll need to
- define some routes to help make the URL in the browser look better
- essentially have 2 sites in the same app
- have a servie that just manages device activity
- do some searching of active record objects
