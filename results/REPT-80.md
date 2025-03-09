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
Test mode:    split 80.0% train, remainder test

=== Evaluation on test split ===

Time taken to test model on test split: 0.07 seconds

=== Summary ===

Correctly Classified Instances       23650               97.5821 %
Incorrectly Classified Instances       586                2.4179 %
Kappa statistic                          0.953 
Mean absolute error                      0.006 
Root mean squared error                  0.0588
Relative absolute error                  7.4445 %
Root relative squared error             29.437  %
Total Number of Instances            24236     

=== Detailed Accuracy By Class ===

                 TP Rate  FP Rate  Precision  Recall   F-Measure  MCC      ROC Area  PRC Area  Class
                 0.993    0.000    0.995      0.993    0.994      0.994    1.000     0.999     Cancelled
                 0.990    0.025    0.923      0.990    0.955      0.942    0.988     0.946     Shipped - Delivered to Buyer
                 1.000    0.000    1.000      1.000    1.000      1.000    1.000     1.000     Shipped
                 0.016    0.002    0.136      0.016    0.029      0.042    0.801     0.076     Shipped - Returned to Seller
                 0.000    0.000    ?          0.000    ?          ?        0.486     0.000     Shipped - Rejected by Buyer
                 0.000    0.000    ?          0.000    ?          ?        0.999     0.026     Shipped - Lost in Transit
                 0.083    0.000    1.000      0.083    0.154      0.289    0.654     0.085     Shipped - Out for Delivery
                 0.000    0.000    ?          0.000    ?          ?        0.753     0.036     Shipped - Returning to Seller
                 0.707    0.001    0.865      0.707    0.778      0.781    0.989     0.723     Shipped - Picked Up
                 0.738    0.002    0.703      0.738    0.720      0.719    0.978     0.734     Pending
                 0.591    0.001    0.667      0.591    0.627      0.627    0.998     0.737     Pending - Waiting for Pick Up
                 ?        0.000    ?          ?        ?          ?        ?         ?         Shipped - Damaged
                 ?        0.000    ?          ?        ?          ?        ?         ?         Shipping
Weighted Avg.    0.976    0.006    ?          0.976    ?          ?        0.993     0.967     

=== Confusion Matrix ===

     	 a     b     c     d     e     f     g     h     i     j     k     l     m   <-- classified as
      2115     0     0     0     0     0     0     0     0    15     0     0     0 |     a = Cancelled
         0  5594     0    37     0     0     0     0    12    10     0     0     0 |     b = Shipped - Delivered to Buyer
         0     0 15690     0     0     0     0     0     0     0     0     0     0 |     c = Shipped
         0   364     0     6     0     0     0     0     0     0     0     0     0 |     d = Shipped - Returned to Seller
         0     2     0     0     0     0     0     0     1     0     0     0     0 |     e = Shipped - Rejected by Buyer
         0     1     0     0     0     0     0     0     0     0     0     0     0 |     f = Shipped - Lost in Transit
         0     8     0     0     0     0     1     0     3     0     0     0     0 |     g = Shipped - Out for Delivery
         0    26     0     1     0     0     0     0     3     0     0     0     0 |     h = Shipped - Returning to Seller
         0    53     0     0     0     0     0     0   128     0     0     0     0 |     i = Shipped - Picked Up
        10     7     2     0     0     0     0     0     0    90    13     0     0 |     j = Pending
         0     4     0     0     0     0     0     0     1    13    26     0     0 |     k = Pending - Waiting for Pick Up
         0     0     0     0     0     0     0     0     0     0     0     0     0 |     l = Shipped - Damaged
         0     0     0     0     0     0     0     0     0     0     0     0     0 |     m = Shipping

