# Calendar

### NOTE: Currently using this app as a staging ground for learning [Shoes](http://shoesrb.com/). Latest commits may have broken parts of the app.

### Usage

Clone the repo.

Run these commands:

    bundle install
    rake db:create db:migrate db:test:prepare
    bundle exec rspec  # ensure all tests pass
    bundle exec ruby calendar.rb

### Create a calendar app.

* **DONE** First, let users create, edit, and delete events with a description, location, and a start and end date and time.
* **DONE** Next, let users list out the events in the order in which they will occur. By default, only list events in the future.
* **DONE** Now, create a view that lets users choose to only view events on the current day, week, or month.
* **DONE** In the day/week/month view, let users choose to view the previous or following day/week/month, so that they can "scroll" through their events.
* **DONE** Add the ability to make generic to-do items that don't have a date or time.
* **DONE** Now, let users add notes to events and to-dos. When you have an object that can belong to more than one class, it's called polymorphic. Read the Rails Guide section on polymorphism to learn how to implement it. This may be a bit tricky at first.
* **DONE** Validate that your events have correct dates and times by using the validates_timeliness gem. validates_timeliness doesn't have good tools for testing, so feel free to skip out on the testing.
* **DONE** Implement full-text search across your event names, descriptions, and locations using the textacular gem.
* **DONE** Allow events to be marked as repeating every day, week, month, or year, and display them appropriately on each view.
