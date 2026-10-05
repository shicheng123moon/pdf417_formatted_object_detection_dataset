# pdf417-formatted barcode object detection dataset
This is a barcode detection dataset for detecting pdf417-formatted barcodes under the shooting of industrial cameras.
This dataset contains 1,416 images with annotations of YOLO format and COCO format offered.
The YOLOv8s model trained by this dataset has been applied in the BatchScan software in Ericsson logistics. 

# Rank and Sort Loss-aware Label Assignment
The recent progress in object detection seeks to design more effective and dynamic label assignment strategies
that automatically select training samples in a prediction-aware manner. In this paper, we revisit the loss-aware label assignment
and innovatively propose the Rank and Sort (RS) Loss-aware Label Assignment with Centroid Prior (RSLLACP), which is
more noise-robust and adapted to the semantic patterns of each instance. By taking advantage of the instance mask annotations,
the centroid prior is more appropriate than the geometric center to define the region for positive anchors due to more
informative features contained within. Besides, the centroid prior prevents the ambiguous anchors from taking place. Inspired by
the recent advances that the ranking-based objective functions can dramatically improve detection performance, RSLLACP
proposes to incorporate the RS cost into the matching cost matrix to replace the classification cost. Thanks to its ranking-based
nature, the positive anchors are differentiated from the negatives by the classification logits while being robust to the foreground-background
class imbalance. Due to its sorting objective, positive anchors are prioritized with respect to their continuous localization qualities. 
This ranking and sorting nature lines up with the label assignment objective. Extensive experiments on the MS COCO dataset validate the effectiveness of our proposed
RSLLACP. Without bells and whistles, RSLLACP achieves 51.9 mAP, outperforming all existing state-of-the-art one-stage detectors by a significant margin.

# Citation
If the dataset inspires you, please cite us:
```
@inproceedings{zu2024, 
   title = {Rank and Sort Loss-Aware Label Assignment with Centroid Prior for Dense Object Detection}, 
   author = {Zu, Shicheng and Jin, Yucheng}, 
   booktitle = {2024 IEEE 18th International Conference on Automatic Face and Gesture Recognition (FG)}, 
   pages={1--9}, 
   year = {2024}
}
```
