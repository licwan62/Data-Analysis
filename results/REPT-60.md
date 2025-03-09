=== Run information ===

Scheme:       weka.classifiers.trees.REPTree -M 2 -V 0.001 -N 3 -S 1 -L -1 -I 0.0
Relation:     Amazon Sale Report - edit-weka.filters.unsupervised.instance.RemoveWithValues-S0.0-C1-Lfirst-last-M-weka.filters.unsupervised.instance.RemoveWithValues-S0.0-C16-L647.62-weka.filters.unsupervised.instance.RemoveWithValues-S0.0-C16-L647.62-weka.filters.unsupervised.instance.RemoveWithValues-S0.0-C16-L647.62-weka.filters.unsupervised.instance.RemoveWithValues-S0.0-C16-Lfirst-last-M-weka.filters.unsupervised.instance.RemoveWithValues-S0.0-C14-L0-M-weka.filters.unsupervised.attribute.MathExpression-Eifelse(A14=0,1,0)-V-weka.filters.unsupervised.attribute.MathExpression-Eifelse(A14=0,1,0)-V-weka.filters.unsupervised.attribute.MathExpression-Eifelse(A14=0,1,0)-V-weka.filters.unsupervised.attribute.MathExpression-Eifelse(A14=0,1,0)-V-weka.filters.unsupervised.attribute.Remove-R1-2
Instances:    121180
Attributes:   22
              Date
              Status
              Fulfilment
              Sales Channel 
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
              ship-state
              ship-postal-code
              ship-country
              promotion-ids
              B2B
              fulfilled-by
              Unnamed: 22
Test mode:    split 60.0% train, remainder test

=== Evaluation on test split ===

Time taken to test model on test split: 0.07 seconds

=== Summary ===

Correctly Classified Instances       47261               97.5017 %
Incorrectly Classified Instances      1211                2.4983 %
Kappa statistic                          0.9517
Mean absolute error                      0.0062
Root mean squared error                  0.0597
Relative absolute error                  7.6914 %
Root relative squared error             29.8063 %
Total Number of Instances            48472     

=== Detailed Accuracy By Class ===

                 TP Rate  FP Rate  Precision  Recall   F-Measure  MCC      ROC Area  PRC Area  Class
                 0.994    0.001    0.994      0.994    0.994      0.993    1.000     0.997     Cancelled
                 0.991    0.026    0.920      0.991    0.955      0.941    0.989     0.945     Shipped - Delivered to Buyer
                 1.000    0.000    1.000      1.000    1.000      1.000    1.000     1.000     Shipped
                 0.013    0.001    0.128      0.013    0.024      0.037    0.794     0.079     Shipped - Returned to Seller
                 0.000    0.000    ?          0.000    ?          ?        0.483     0.000     Shipped - Rejected by Buyer
                 0.000    0.000    ?          0.000    ?          ?        0.999     0.076     Shipped - Lost in Transit
                 0.067    0.000    1.000      0.067    0.125      0.258    0.651     0.068     Shipped - Out for Delivery
                 0.033    0.000    0.182      0.033    0.056      0.077    0.734     0.034     Shipped - Returning to Seller
                 0.636    0.001    0.856      0.636    0.730      0.736    0.985     0.655     Shipped - Picked Up
                 0.710    0.001    0.744      0.710    0.727      0.725    0.941     0.744     Pending
                 0.477    0.001    0.667      0.477    0.556      0.563    0.977     0.545     Pending - Waiting for Pick Up
                 0.000    0.000    ?          0.000    ?          ?        0.500     0.000     Shipped - Damaged
                 ?        0.000    ?          ?        ?          ?        ?         ?         Shipping
Weighted Avg.    0.975    0.006    ?          0.975    ?          ?        0.993     0.966     

=== Confusion Matrix ===

     a     b     c     d     e     f     g     h     i     j     k     l     m   <-- classified as
  4230     0     0     0     0     0     0     0     0    25     0     0     0 |     a = Cancelled
     0 11320     0    67     0     0     0     4    27     1     0     0     0 |     b = Shipped - Delivered to Buyer
     0     0 31234     0     0     0     0     0     0     0     0     0     0 |     c = Shipped
     0   743     0    10     0     0     0     0     1     0     0     0     0 |     d = Shipped - Returned to Seller
     0     4     0     0     0     0     0     0     0     0     0     0     0 |     e = Shipped - Rejected by Buyer
     0     2     0     0     0     0     0     0     0     0     0     0     0 |     f = Shipped - Lost in Transit
     0    10     0     0     0     0     1     0     4     0     0     0     0 |     g = Shipped - Out for Delivery
     0    52     0     1     0     0     0     2     5     0     0     0     0 |     h = Shipped - Returning to Seller
     0   131     0     0     0     0     0     5   238     0     0     0     0 |     i = Shipped - Picked Up
    27    16     2     0     0     0     0     0     0   174    26     0     0 |     j = Pending
     0    20     0     0     0     0     0     0     3    34    52     0     0 |     k = Pending - Waiting for Pick Up
     0     1     0     0     0     0     0     0     0     0     0     0     0 |     l = Shipped - Damaged
     0     0     0     0     0     0     0     0     0     0     0     0     0 |     m = Shipping

