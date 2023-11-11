# GAE-R: GAE Related Models and Evaluations

For table1 evaluation:
sh Table-1.sh

For table2&3&4 evaluation:
sh Table-234.sh

Ref of tables: 
1. {CQR, CP, QR}× {DiGAE, GAE, LGNN}× {coverage, ineff iciency} (use
GraphConv or SAGEConv as the graph convolutional layer, use ”CQR” as
the score). Conclusion: QR does not meet the coverage requirement, while
CQR and CP do.
2. {CQR, CP}×{DiGAE, GAE, LGNN}×{GraphConv, GCNConv, SAGEConv, GAT Conv}×
{coveragex
, ineff iciency}. Conclusion: No matter what graph convolutional
layers we choose, DiGAE/GAE outperforms LGNN, CQR outperforms CP.
3. {CQR, CP}×{DiGAE, GAE}×{GraphConv, GCNConv}×{coveragex
, ineff iciency}.
Conclusion: Adding the usage of edge weight is better than only use edge
index.
4. CQR×{DiGAE, GAE, LGNN}×{GraphConv, GCNConv, SAGEConv, GAT Conv}×
{coveragex
, ineff iciency} × {”CQR”, ”CQR − new”}. Conclusion: ”CQRnew” outperforms
 ”CQR” scoring method.
