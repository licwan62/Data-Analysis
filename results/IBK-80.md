=== Run information ===

Scheme:       weka.classifiers.lazy.IBk -K 1 -W 0 -A "weka.core.neighboursearch.LinearNNSearch -A \"weka.core.EuclideanDistance -R first-last\""
Relation:     Amazon Sale Report-weka.filters.unsupervised.instance.RemoveWithValues-S0.0-C1-Lfirst-last-M-weka.filters.unsupervised.instance.RemoveWithValues-S0.0-C16-L647.62-weka.filters.unsupervised.instance.RemoveWithValues-S0.0-C16-L647.62-weka.filters.unsupervised.instance.RemoveWithValues-S0.0-C16-L647.62-weka.filters.unsupervised.instance.RemoveWithValues-S0.0-C16-Lfirst-last-M-weka.filters.unsupervised.instance.RemoveWithValues-S0.0-C14-L0-M-weka.filters.unsupervised.attribute.MathExpression-Eifelse(A14=0,1,0)-V-weka.filters.unsupervised.attribute.MathExpression-Eifelse(A14=0,1,0)-V-weka.filters.unsupervised.attribute.MathExpression-Eifelse(A14=0,1,0)-V-weka.filters.unsupervised.attribute.MathExpression-Eifelse(A14=0,1,0)-V-weka.filters.unsupervised.attribute.Remove-R1-2-weka.filters.unsupervised.attribute.Remove-R19-weka.filters.unsupervised.attribute.Remove-R4,16-17,20-21
Instances:    121180
Attributes:   16
              Date
              Status
              Fulfilment
              ship-service-level
              Style
              SKU
              Category
              Size
              ASIN
              Courier Status
              Qty
              currency
              Amount
              ship-city
              ship-country
              B2B
Test mode:    split 80.0% train, remainder test

=== Classifier model (full training set) ===

IB1 instance-based classifier
using 1 nearest neighbour(s) for classification


Time taken to build model: 0.01 seconds

=== Evaluation on test split ===

Time taken to test model on test split: 149.64 seconds

=== Summary ===

Correctly Classified Instances       21893               90.3326 %
Incorrectly Classified Instances      2343                9.6674 %
Kappa statistic                          0.8076
Mean absolute error                      0.0169
Root mean squared error                  0.1211
Relative absolute error                 21.0076 %
Root relative squared error             60.6295 %
Total Number of Instances            24236     

=== Detailed Accuracy By Class ===

                 TP Rate  FP Rate  Precision  Recall   F-Measure  MCC      ROC Area  PRC Area  Class
                 0.491    0.012    0.802      0.491    0.609      0.601    0.840     0.515     Cancelled
                 0.932    0.059    0.828      0.932    0.877      0.839    0.955     0.816     Shipped - Delivered to Buyer
                 0.987    0.079    0.958      0.987    0.972      0.920    0.975     0.977     Shipped
                 0.030    0.008    0.055      0.030    0.039      0.030    0.589     0.025     Shipped - Returned to Seller
                 0.000    0.000    0.000      0.000    0.000      -0.000   0.798     0.000     Shipped - Rejected by Buyer
                 0.000    0.000    ?          0.000    ?          ?        0.510     0.000     Shipped - Lost in Transit
                 0.083    0.000    0.200      0.083    0.118      0.129    0.516     0.017     Shipped - Out for Delivery
                 0.000    0.001    0.000      0.000    0.000      -0.001   0.557     0.003     Shipped - Returning to Seller
                 0.254    0.003    0.400      0.254    0.311      0.315    0.718     0.173     Shipped - Picked Up
                 0.213    0.001    0.456      0.213    0.291      0.309    0.656     0.144     Pending
                 0.318    0.000    0.560      0.318    0.406      0.421    0.743     0.217     Pending - Waiting for Pick Up
                 ?        0.000    ?          ?        ?          ?        ?         ?         Shipped - Damaged
                 ?        0.000    ?          ?        ?          ?        ?         ?         Shipping
Weighted Avg.    0.903    0.066    ?          0.903    ?          ?        0.948     0.871     

=== Confusion Matrix ===

     	a     b     c     d     e     f     g     h     i     j     k     l     m   <-- classified as
      1046   493   525    26     0     0     1     0    18    17     4     0     0 |     a = Cancelled
        68  5267   104   153     3     0     3    10    44     1     0     0     0 |     b = Shipped - Delivered to Buyer
       146    48 15482     4     0     0     0     1     1     8     0     0     0 |     c = Shipped
         1   352     5    11     0     0     0     0     1     0     0     0     0 |     d = Shipped - Returned to Seller
         0     1     1     1     0     0     0     0     0     0     0     0     0 |     e = Shipped - Rejected by Buyer
         0     1     0     0     0     0     0     0     0     0     0     0     0 |     f = Shipped - Lost in Transit
         0     8     0     1     0     0     1     0     2     0     0     0     0 |     g = Shipped - Out for Delivery
         0    29     0     0     0     0     0     0     1     0     0     0     0 |     h = Shipped - Returning to Seller
         2   119     7     2     1     0     0     3    46     0     1     0     0 |     i = Shipped - Picked Up
        40    19    29     1     0     0     0     0     1    26     6     0     0 |     j = Pending
         2    22     0     0     0     0     0     0     1     5    14     0     0 |     k = Pending - Waiting for Pick Up
         0     0     0     0     0     0     0     0     0     0     0     0     0 |     l = Shipped - Damaged
         0     0     0     0     0     0     0     0     0     0     0     0     0 |     m = Shipping
    
    
