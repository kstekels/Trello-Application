# Trello
Develop iOS application using [Trello API](https://developers.trello.com/docs/api-introduction). First, **Boards** scene, will present view to authorize with Trello, afterwards, will display all boards signed-in user has. User can filter boards using search bar. Selecting board will navigate user to second scene which displays **Board** details - lists and corresponding cards with labels. When selecting card user is navigated to **Card** details scene where labels are popolated with their titles, text view is shows current card description or a placeholder. If user edits text view and taps save it will send update to Trello. If user taps delete on card, alert will be presented with descriptive message, if user proceeds card will be deleted from Trello.

### Recources:
- [Prototype](https://invis.io/GQRR3B65P2E);
- [Designs](https://zpl.io/VYr1Lom);
- [Trello API](https://developers.trello.com/docs/api-introduction);
- [Assets](https://trello-attachments.s3.amazonaws.com/5cacdd2a6b0bdc3698b3b195/5cb62aec119a4d6c3e0b515c/cb2fc3be01f3b084064eb1e2d3e1e688/assets.zip);
- [`SFSafariViewController`](https://developer.apple.com/documentation/safariservices/sfsafariviewcontroller);
- [`UINavigationController`](https://developer.apple.com/documentation/uikit/uinavigationcontroller);
- [`UITableView`](https://developer.apple.com/documentation/uikit/uitableview);
- [`UICollectionView`](https://developer.apple.com/documentation/uikit/uicollectionview);
- [`UITextView`](https://developer.apple.com/documentation/uikit/uitextview).

### Workflow:
- Create a repository;
- Create branch `develop` of `main` branch;
- Split assignment in multiple components and/or steps (_e.g.,_ set-up environment, create user interface, implement fetching of user location, add networking layer, fetch weather data for current day, fetch weather forcaset for future days _etc._);
- For each component you will create seperate branch (_e.g.,_ `component-x` branch), **one-at-a-time**, push changes to that branch and create pull request from `component-x` branch to `develop` branch. This way each component will be reviewed seperately inside pull request and `develop` branch will have only clean, reviewed code which will eventually build-up to complete application and will be merged to `main` as a release.

### Tips:
- Upon successful authorization with Trello API, token will be received via [`application(_:open:options:)`](https://developer.apple.com/documentation/uikit/uiapplicationdelegate/1623112-application) in `AppDelegate` class. Token will be part of `URL` accessible via `url` parameter;
- Use **InVision** [prototype](https://invis.io/GQRR3B65P2E) to get a general idea of transitions and view controller hierarchy;
- Use **Zeplin** [designs](https://zpl.io/VYr1Lom) to get exact spacings between elements, sizes of objects, fonts and colors (in more difficult components designs do not have to be pixel perfect, but have to be close);
- Drag and drop [assets](https://trello-attachments.s3.amazonaws.com/5cacdd2a6b0bdc3698b3b195/5cb62aec119a4d6c3e0b515c/cb2fc3be01f3b084064eb1e2d3e1e688/assets.zip) to `Assets.xcassets` of project.
