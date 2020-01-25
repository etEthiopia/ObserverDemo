What is Observer Pattern?

    Observer Pattern is a pattern in which an object, called the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.

Components

    1. Subject

    2. MyTopic

    3. MyTopicSubscriber

    4. Observer

    5. ObserverPatternExample

1. Subject

   Contains the structure including
   register(observer)
   unregister(observer)
   notifyObservers()
   getUpdate(observer)

2 MyTopic

    It implements Subject and overrides the methods.
    It includes a List of Observers

3. Observer

   An Interface with methods like 'update' and 'setSubject'

4) MyTopicSubscriber

   implements Observer
   Which has 'name' and 'topic'
   It overrides the 'update' method and set the Subject
