---
currentMenu: events
---

# Events

BoomCMS makes use of [Laravel's event classes](http://laravel.com/docs/5.1/events) making it easy for developers to extend CMS functionality.

Before reading this section you should be familiar with Laravel events, in particular how to listen for and respond to events, by reading the Event documentation at http://laravel.com/docs/5.1/events

Event classes can be found in the [BoomCMS\Events](https://github.com/boomcms/boom-core/tree/master/src/BoomCMS/Events) namespace.
BoomCMS fires these events after certain actions:

## Page Events

Action | Notes | Event class
------ | ------ | ------
Page created | | [BoomCMS\Events\PageWasCreated](https://github.com/boomcms/boom-core/tree/master/src/BoomCMS/Events/PageWasCreated.php)
Approval requested for page drafts | | [BoomCMS\Events\PageApprovalRequested](https://github.com/boomcms/boom-core/tree/master/src/BoomCMS/Events/PageApprovalRequested.php)
Page template changed | | [BoomCMS\Events\PageTemplateChanged](https://github.com/boomcms/boom-core/tree/master/src/BoomCMS/Events/PageTemplateWasChanged.php)
Page title changed | | [BoomCMS\Events\PageTitleWasChanged](https://github.com/boomcms/boom-core/tree/master/src/BoomCMS/Events/PageTitleWasChanged.php)
Page deleted | | [BoomCMS\Events\PageWasDeleted](https://github.com/boomcms/boom-core/tree/master/src/BoomCMS/Events/PageWasDeleted.php)
Page made visible | Event fired when an invisible page has it's visibility setting changed to 'visible' | [BoomCMS\Events\PageWasMadeVisible](https://github.com/boomcms/boom-core/tree/master/src/BoomCMS/Events/PageWasMadeVisible.php)
Page published | Events fired when a page version is set to be published. Won't be fired if changes are embargoed | [BoomCMS\Events\PageWasPublished](https://github.com/boomcms/boom-core/tree/master/src/BoomCMS/Events/PageWasPublished.php)
Chunk created | Fired when chunk content is saved (i.e. a new version of a chunk is created | [BoomCMS\Events\ChunkWasCreated](https://github.com/boomcms/boom-core/tree/master/src/BoomCMS/Events/ChunkWasCreated.php)

## Authentication Events
Action | Event class
------ | ------
Failed Login | [BoomCMS\Events\FailedLogin](https://github.com/boomcms/boom-core/tree/master/src/BoomCMS/Events/FailedLogin.php)
Successful Login | [BoomCMS\Events\SuccessfulLogin](https://github.com/boomcms/boom-core/tree/master/src/BoomCMS/Events/SucessfulLogin.php)
Logout | [BoomCMS\Events\Logout](https://github.com/boomcms/boom-core/tree/master/src/BoomCMS/Events/Logout.php)