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
Test mode:    split 60.0% train, remainder test

=== Evaluation on test split ===

Time taken to test model on test split: 0.42 seconds

=== Summary ===

Correctly Classified Instances       46942               96.8435 %
Incorrectly Classified Instances      1530                3.1565 %
Kappa statistic                          0.939 
Mean absolute error                      0.0065
Root mean squared error                  0.0649
Relative absolute error                  8.0167 %
Root relative squared error             32.4016 %
Total Number of Instances            48472     

=== Detailed Accuracy By Class ===

                 TP Rate  FP Rate  Precision  Recall   F-Measure  MCC      ROC Area  PRC Area  Class
                 0.944    0.002    0.978      0.944    0.961      0.957    0.999     0.972     Cancelled
                 0.977    0.030    0.910      0.977    0.943      0.925    0.989     0.942     Shipped - Delivered to Buyer
                 1.000    0.001    0.999      1.000    0.999      0.998    1.000     1.000     Shipped
                 0.034    0.004    0.112      0.034    0.053      0.054    0.880     0.074     Shipped - Returned to Seller
                 0.000    0.000    0.000      0.000    0.000      -0.000   0.817     0.000     Shipped - Rejected by Buyer
                 0.000    0.000    0.000      0.000    0.000      -0.000   0.829     0.000     Shipped - Lost in Transit
                 0.000    0.000    0.000      0.000    0.000      -0.000   0.901     0.003     Shipped - Out for Delivery
                 0.000    0.000    0.000      0.000    0.000      -0.001   0.945     0.025     Shipped - Returning to Seller
                 0.722    0.001    0.833      0.722    0.774      0.774    0.994     0.830     Shipped - Picked Up
                 0.747    0.001    0.863      0.747    0.801      0.802    0.994     0.841     Pending
                 0.642    0.000    0.909      0.642    0.753      0.764    1.000     0.880     Pending - Waiting for Pick Up
                 0.000    0.000    ?          0.000    ?          ?        0.738     0.000     Shipped - Damaged
                 ?        0.000    ?          ?        ?          ?        ?         ?         Shipping
Weighted Avg.    0.968    0.008    ?          0.968    ?          ?        0.995     0.965     

=== Confusion Matrix ===

     a     b     c     d     e     f     g     h     i     j     k     l     m   <-- classified as
  4016   199     8     3     0     0     0     0     2    27     0     0     0 |     a = Cancelled
     5 11157     0   200     3     0     4     9    41     0     0     0     0 |     b = Shipped - Delivered to Buyer
     8     1 31220     0     0     2     1     1     1     0     0     0     0 |     c = Shipped
     2   726     0    26     0     0     0     0     0     0     0     0     0 |     d = Shipped - Returned to Seller
     0     3     0     0     0     0     0     0     1     0     0     0     0 |     e = Shipped - Rejected by Buyer
     0     2     0     0     0     0     0     0     0     0     0     0     0 |     f = Shipped - Lost in Transit
     0    10     0     1     0     0     0     1     3     0     0     0     0 |     g = Shipped - Out for Delivery
     0    52     0     2     0     0     0     0     6     0     0     0     0 |     h = Shipped - Returning to Seller
     0   103     0     0     0     0     0     1   270     0     0     0     0 |     i = Shipped - Picked Up
    39     0    16     0     0     0     0     0     0   183     7     0     0 |     j = Pending
    37     0     0     0     0     0     0     0     0     2    70     0     0 |     k = Pending - Waiting for Pick Up
     0     1     0     0     0     0     0     0     0     0     0     0     0 |     l = Shipped - Damaged
     0     0     0     0     0     0     0     0     0     0     0     0     0 |     m = Shipping

