# Cell-Spacing-Manage-for-CollectionView

Firstly mention your spacing

    var cellSpace = CGFloat(3)
    
## Now set the flow layout UICollectionViewDelegateFlowLayout function
    
    func collectionView(_ collectionView: UICollectionView, layout collectionViewLayout: UICollectionViewLayout, sizeForItemAt indexPath: IndexPath) -> CGSize {
        
        let width  = Int(imgCollectionView.frame.size.width/4)-Int(cellSpace)
        
        return CGSize(width: width, height: width)
    }
    
## Now use spacing method 
  
    func collectionView(_ collectionView: UICollectionView, layout collectionViewLayout: UICollectionViewLayout, minimumInteritemSpacingForSectionAt section: Int) -> CGFloat {
          return cellSpace
      }
      
      func collectionView(_ collectionView: UICollectionView, layout collectionViewLayout: UICollectionViewLayout, minimumLineSpacingForSectionAt section: Int) -> CGFloat {
          return cellSpace
      }
Now Run project :D 


<img src="https://user-images.githubusercontent.com/29371886/123251903-8655e780-d50d-11eb-9c68-f03673c30a1e.png" 
     width="400" 
     height="500" />

