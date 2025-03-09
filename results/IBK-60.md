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
Test mode:    split 60.0% train, remainder test

=== Classifier model (full training set) ===

IB1 instance-based classifier
using 1 nearest neighbour(s) for classification


Time taken to build model: 0.03 seconds

=== Evaluation on test split ===

Time taken to test model on test split: 199.79 seconds

=== Summary ===

Correctly Classified Instances       43390               89.5156 %
Incorrectly Classified Instances      5082               10.4844 %
Kappa statistic                          0.7922
Mean absolute error                      0.018 
Root mean squared error                  0.1259
Relative absolute error                 22.3198 %
Root relative squared error             62.8694 %
Total Number of Instances            48472     

=== Detailed Accuracy By Class ===

                 TP Rate  FP Rate  Precision  Recall   F-Measure  MCC      ROC Area  PRC Area  Class
                 0.473    0.013    0.773      0.473    0.587      0.577    0.823     0.480     Cancelled
                 0.914    0.062    0.820      0.914    0.864      0.822    0.949     0.804     Shipped - Delivered to Buyer
                 0.984    0.087    0.953      0.984    0.968      0.910    0.969     0.972     Shipped
                 0.034    0.008    0.062      0.034    0.044      0.035    0.597     0.027     Shipped - Returned to Seller
                 0.000    0.000    0.000      0.000    0.000      -0.000   0.707     0.000     Shipped - Rejected by Buyer
                 0.000    0.000    0.000      0.000    0.000      -0.000   0.632     0.000     Shipped - Lost in Transit
                 0.067    0.000    0.111      0.067    0.083      0.086    0.537     0.008     Shipped - Out for Delivery
                 0.017    0.001    0.028      0.017    0.021      0.021    0.574     0.002     Shipped - Returning to Seller
                 0.222    0.003    0.337      0.222    0.268      0.269    0.682     0.132     Shipped - Picked Up
                 0.212    0.001    0.441      0.212    0.287      0.303    0.653     0.138     Pending
                 0.367    0.000    0.702      0.367    0.482      0.507    0.727     0.295     Pending - Waiting for Pick Up
                 0.000    0.000    ?          0.000    ?          ?        0.205     0.000     Shipped - Damaged
                 ?        0.000    ?          ?        ?          ?        ?         ?         Shipping
Weighted Avg.    0.895    0.072    ?          0.895    ?          ?        0.940     0.861     

=== Confusion Matrix ===

     	a     b     c     d     e     f     g     h     i     j     k     l     m   <-- classified as
      2011  1022  1105    44     0     0     2     2    28    38     3     0     0 |     a = Cancelled
       187 10442   300   335     5     0     5    21   116     5     3     0     0 |     b = Shipped - Delivered to Buyer
       308   162 30734     7     0     1     0     1     5    16     0     0     0 |     c = Shipped
        10   692    18    26     0     0     0     3     5     0     0     0     0 |     d = Shipped - Returned to Seller
         0     2     1     1     0     0     0     0     0     0     0     0     0 |     e = Shipped - Rejected by Buyer
         0     2     0     0     0     0     0     0     0     0     0     0     0 |     f = Shipped - Lost in Transit
         0    10     0     1     0     0     1     1     2     0     0     0     0 |     g = Shipped - Out for Delivery
         0    51     6     0     0     0     1     1     1     0     0     0     0 |     h = Shipped - Returning to Seller
         8   259    14     4     1     0     0     5    83     0     0     0     0 |     i = Shipped - Picked Up
        75    46    59     1     0     0     0     0     1    52    11     0     0 |     j = Pending
         2    52     0     1     0     0     0     2     5     7    40     0     0 |     k = Pending - Waiting for Pick Up
         0     1     0     0     0     0     0     0     0     0     0     0     0 |     l = Shipped - Damaged
         0     0     0     0     0     0     0     0     0     0     0     0     0 |     m = Shipping
    
    
