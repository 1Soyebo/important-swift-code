# important-swift-code
Important Swift Code and Markdown Practice

```swift
  public override func willTransition(to newCollection: UITraitCollection, with coordinator: UIViewControllerTransitionCoordinator) {
        if UIDevice.current.orientation.isLandscape,
            let layout = collectionView.collectionViewLayout as? UICollectionViewFlowLayout {
            let width = view.frame.height - 22
            layout.itemSize = CGSize(width: width - 16, height: 160)
            layout.invalidateLayout()
        } else if UIDevice.current.orientation.isPortrait,
            let layout = collectionView.collectionViewLayout as? UICollectionViewFlowLayout {
            let width = view.frame.width - 22
            layout.itemSize = CGSize(width: width - 16, height: 160)
            layout.invalidateLayout()
        }
    }
```
