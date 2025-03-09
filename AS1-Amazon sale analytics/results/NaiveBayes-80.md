=== Run information ===

Scheme:       weka.classifiers.bayes.NaiveBayes 
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
Test mode:    split 80.0% train, remainder test

=== Evaluation on test split ===

Time taken to test model on test split: 0.19 seconds

=== Summary ===

Correctly Classified Instances       23478               96.8724 %
Incorrectly Classified Instances       758                3.1276 %
Kappa statistic                          0.9393
Mean absolute error                      0.0063
Root mean squared error                  0.0641
Relative absolute error                  7.8687 %
Root relative squared error             32.0952 %
Total Number of Instances            24236     

=== Detailed Accuracy By Class ===

                 TP Rate  FP Rate  Precision  Recall   F-Measure  MCC      ROC Area  PRC Area  Class
                 0.940    0.002    0.980      0.940    0.960      0.956    0.999     0.975     Cancelled
                 0.975    0.029    0.911      0.975    0.942      0.924    0.989     0.944     Shipped - Delivered to Buyer
                 1.000    0.001    1.000      1.000    1.000      0.999    1.000     1.000     Shipped
                 0.024    0.005    0.072      0.024    0.036      0.033    0.881     0.072     Shipped - Returned to Seller
                 0.000    0.000    0.000      0.000    0.000      -0.000   0.827     0.001     Shipped - Rejected by Buyer
                 0.000    0.000    ?          0.000    ?          ?        0.962     0.001     Shipped - Lost in Transit
                 0.000    0.000    0.000      0.000    0.000      -0.000   0.900     0.006     Shipped - Out for Delivery
                 0.033    0.000    0.167      0.033    0.056      0.074    0.944     0.036     Shipped - Returning to Seller
                 0.812    0.001    0.845      0.812    0.828      0.827    0.997     0.882     Shipped - Picked Up
                 0.787    0.001    0.865      0.787    0.824      0.824    0.993     0.842     Pending
                 0.614    0.000    0.900      0.614    0.730      0.743    1.000     0.839     Pending - Waiting for Pick Up
                 ?        0.000    ?          ?        ?          ?        ?         ?         Shipped - Damaged
                 ?        0.000    ?          ?        ?          ?        ?         ?         Shipping
Weighted Avg.    0.969    0.007    ?          0.969    ?          ?        0.995     0.967     

=== Confusion Matrix ===

     a     b     c     d     e     f     g     h     i     j     k     l     m   <-- classified as
  2002   113     0     0     0     0     0     0     1    14     0     0     0 |     a = Cancelled
     3  5511     0   113     1     0     2     3    20     0     0     0     0 |     b = Shipped - Delivered to Buyer
     3     0 15685     0     0     0     2     0     0     0     0     0     0 |     c = Shipped
     1   360     0     9     0     0     0     0     0     0     0     0     0 |     d = Shipped - Returned to Seller
     0     2     0     0     0     0     0     0     1     0     0     0     0 |     e = Shipped - Rejected by Buyer
     0     1     0     0     0     0     0     0     0     0     0     0     0 |     f = Shipped - Lost in Transit
     0     8     0     1     0     0     0     1     2     0     0     0     0 |     g = Shipped - Out for Delivery
     0    24     0     2     0     0     0     1     3     0     0     0     0 |     h = Shipped - Returning to Seller
     0    33     0     0     0     0     0     1   147     0     0     0     0 |     i = Shipped - Picked Up
    17     0     6     0     0     0     0     0     0    96     3     0     0 |     j = Pending
    16     0     0     0     0     0     0     0     0     1    27     0     0 |     k = Pending - Waiting for Pick Up
     0     0     0     0     0     0     0     0     0     0     0     0     0 |     l = Shipped - Damaged
     0     0     0     0     0     0     0     0     0     0     0     0     0 |     m = Shipping

