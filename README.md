# Cell-Spacing-Manage-for-CollectionView

## set the UICollectionViewDelegateFlowLayout function





 func collectionView(_ collectionView: UICollectionView, layout collectionViewLayout: UICollectionViewLayout, sizeForItemAt indexPath: IndexPath) -> CGSize {
        let width  = Int(imgCollectionView.frame.size.width/4)-Int(cellSpace)
        return CGSize(width: width, height: width)
    }
