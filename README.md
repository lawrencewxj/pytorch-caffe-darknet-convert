# caffe-darknet-convert
python caffe2darknet.py ResNet-50-deploy.prototxt

# Todo
- [x] convert prototxt to cfg
- [x] print cfg nicely
- [ ] load caffemodel
- [ ] convert caffemodel to darknet weights

# convert kaiming's resnet50 from caffe to darknet
```
1. download resnet50 from https://github.com/KaimingHe/deep-residual-networks
2. 
```

# convert resnet50 from pytorch to darknet
```
1. python pytorch2darknet.py 
2. python main.py -a resnet50 --pretrained -e /home/xiaohang/ImageNet/
=> using pre-trained model 'resnet50'
load weights from resnet50.weights
Test: [0/196]   Time 16.132 (16.132)    Loss 6.1005 (6.1005)    Prec@1 87.109 (87.109)  Prec@5 97.266 (97.266)
Test: [10/196]  Time 0.387 (1.803)      Loss 6.2117 (6.1357)    Prec@1 77.734 (82.670)  Prec@5 91.797 (95.455)
Test: [20/196]  Time 0.275 (1.261)      Loss 6.1050 (6.1402)    Prec@1 84.375 (82.236)  Prec@5 92.969 (95.424)
Test: [30/196]  Time 0.162 (1.123)      Loss 6.1675 (6.1257)    Prec@1 80.469 (83.543)  Prec@5 95.312 (95.817)
Test: [40/196]  Time 0.889 (1.024)      Loss 6.1888 (6.1483)    Prec@1 81.250 (82.012)  Prec@5 96.875 (95.770)
Test: [50/196]  Time 0.164 (0.970)      Loss 6.0900 (6.1520)    Prec@1 88.281 (81.794)  Prec@5 97.656 (95.956)
Test: [60/196]  Time 0.380 (0.933)      Loss 6.1949 (6.1566)    Prec@1 76.172 (81.416)  Prec@5 93.359 (95.946)
Test: [70/196]  Time 0.427 (0.916)      Loss 6.2009 (6.1525)    Prec@1 78.516 (81.679)  Prec@5 96.484 (96.099)
Test: [80/196]  Time 0.910 (0.900)      Loss 6.3763 (6.1584)    Prec@1 60.938 (81.134)  Prec@5 88.672 (95.751)
Test: [90/196]  Time 1.035 (0.896)      Loss 6.4143 (6.1703)    Prec@1 55.078 (80.039)  Prec@5 86.328 (95.175)
Test: [100/196] Time 0.162 (0.871)      Loss 6.3073 (6.1831)    Prec@1 68.359 (78.968)  Prec@5 91.406 (94.609)
Test: [110/196] Time 0.658 (0.867)      Loss 6.1750 (6.1885)    Prec@1 76.953 (78.442)  Prec@5 94.922 (94.327)
Test: [120/196] Time 0.165 (0.861)      Loss 6.2904 (6.1919)    Prec@1 71.094 (78.141)  Prec@5 88.281 (94.034)
Test: [130/196] Time 1.751 (0.858)      Loss 6.1702 (6.2008)    Prec@1 81.250 (77.290)  Prec@5 94.141 (93.702)
Test: [140/196] Time 0.163 (0.849)      Loss 6.2442 (6.2045)    Prec@1 75.000 (76.948)  Prec@5 90.625 (93.448)
Test: [150/196] Time 2.031 (0.846)      Loss 6.1890 (6.2082)    Prec@1 76.953 (76.604)  Prec@5 91.016 (93.189)
Test: [160/196] Time 0.161 (0.837)      Loss 6.1399 (6.2109)    Prec@1 86.719 (76.366)  Prec@5 94.531 (92.998)
Test: [170/196] Time 1.687 (0.835)      Loss 6.1388 (6.2159)    Prec@1 82.812 (75.959)  Prec@5 97.656 (92.848)
Test: [180/196] Time 1.185 (0.828)      Loss 6.3454 (6.2198)    Prec@1 68.750 (75.650)  Prec@5 91.797 (92.705)
Test: [190/196] Time 1.367 (0.826)      Loss 6.3394 (6.2196)    Prec@1 67.188 (75.685)  Prec@5 95.703 (92.752)
 * Prec@1 75.794 Prec@5 92.798
```

# convert resnet18
```
1. Download resnet18 from https://github.com/HolmesShuan/ResNet-18-Caffemodel-on-ImageNet.git and save as resnet-18.caffemodel
python main.py -a resnet18-caffe --pretrained -e /home/xiaohang/ImageNet/                       
=> using pre-trained model 'resnet18-caffe'
load weights from resnet-18.caffemodel
Loading caffemodel:  resnet-18.caffemodel
Test: [0/196]   Time 26.190 (26.190)    Loss 4.0715 (4.0715)    Prec@1 46.094 (46.094)  Prec@5 69.141 (69.141)
Test: [10/196]  Time 0.224 (2.906)      Loss 3.4033 (3.8355)    Prec@1 44.531 (48.970)  Prec@5 80.078 (77.202)
Test: [20/196]  Time 0.224 (1.970)      Loss 2.6164 (3.2206)    Prec@1 63.672 (54.371)  Prec@5 82.031 (80.283)
Test: [30/196]  Time 0.226 (1.741)      Loss 2.5001 (3.0542)    Prec@1 61.328 (56.074)  Prec@5 89.453 (81.099)
Test: [40/196]  Time 0.134 (1.557)      Loss 3.8292 (3.3356)    Prec@1 42.188 (53.306)  Prec@5 78.516 (79.573)
Test: [50/196]  Time 0.444 (1.485)      Loss 1.7084 (3.4501)    Prec@1 69.531 (51.754)  Prec@5 92.578 (79.059)
Test: [60/196]  Time 0.241 (1.430)      Loss 2.8731 (3.3957)    Prec@1 54.688 (51.992)  Prec@5 80.859 (79.438)
Test: [70/196]  Time 0.202 (1.396)      Loss 2.0834 (3.2644)    Prec@1 66.406 (53.323)  Prec@5 87.109 (80.210)
Test: [80/196]  Time 0.203 (1.357)      Loss 3.3115 (3.2341)    Prec@1 50.781 (53.342)  Prec@5 76.562 (80.295)
Test: [90/196]  Time 1.116 (1.324)      Loss 4.2364 (3.2489)    Prec@1 41.797 (53.280)  Prec@5 71.094 (79.842)
Test: [100/196] Time 0.200 (1.291)      Loss 3.2269 (3.2853)    Prec@1 49.219 (52.943)  Prec@5 76.172 (79.359)
Test: [110/196] Time 1.210 (1.277)      Loss 2.3854 (3.2734)    Prec@1 62.891 (53.167)  Prec@5 83.984 (79.318)
Test: [120/196] Time 1.484 (1.280)      Loss 3.2796 (3.2547)    Prec@1 56.250 (53.454)  Prec@5 75.781 (79.177)
Test: [130/196] Time 3.403 (1.266)      Loss 1.7630 (3.2657)    Prec@1 73.438 (53.232)  Prec@5 90.234 (78.960)
Test: [140/196] Time 1.067 (1.248)      Loss 2.7910 (3.2501)    Prec@1 57.812 (53.433)  Prec@5 80.859 (79.017)
Test: [150/196] Time 1.782 (1.234)      Loss 2.5301 (3.2540)    Prec@1 63.672 (53.498)  Prec@5 81.250 (78.922)
Test: [160/196] Time 1.015 (1.222)      Loss 2.1617 (3.2481)    Prec@1 67.578 (53.470)  Prec@5 84.375 (78.906)
Test: [170/196] Time 0.594 (1.223)      Loss 1.8699 (3.2633)    Prec@1 72.266 (53.388)  Prec@5 91.406 (78.733)
Test: [180/196] Time 1.826 (1.217)      Loss 6.2149 (3.2853)    Prec@1 26.172 (53.149)  Prec@5 49.219 (78.468)
Test: [190/196] Time 1.070 (1.212)      Loss 4.3020 (3.4285)    Prec@1 39.062 (52.090)  Prec@5 66.797 (77.094)
 * Prec@1 51.902 Prec@5 76.834
2. python caffe2darknet.py resnet-18.prototxt resnet-18.caffemodel resnet-18.cfg resnet-18.weights
3. python main.py -a resnet18-darknet --pretrained -e /home/xiaohang/ImageNet/
=> using pre-trained model 'resnet18'
load weights from resnet-18.weights
Test: [0/196]   Time 14.573 (14.573)    Loss 2.5307 (2.5307)    Prec@1 46.484 (46.484)  Prec@5 69.922 (69.922)
Test: [10/196]  Time 0.384 (1.729)      Loss 1.9900 (2.1642)    Prec@1 48.438 (50.036)  Prec@5 81.641 (78.232)
Test: [20/196]  Time 0.292 (1.283)      Loss 1.6162 (1.8913)    Prec@1 68.359 (55.394)  Prec@5 83.203 (81.548)
Test: [30/196]  Time 0.420 (1.186)      Loss 1.4610 (1.8192)    Prec@1 63.672 (56.918)  Prec@5 91.016 (82.271)
Test: [40/196]  Time 0.926 (1.111)      Loss 2.1566 (1.9333)    Prec@1 44.531 (54.059)  Prec@5 80.469 (80.564)
Test: [50/196]  Time 0.154 (1.078)      Loss 1.1988 (1.9701)    Prec@1 68.359 (52.497)  Prec@5 93.359 (80.170)
Test: [60/196]  Time 0.280 (1.043)      Loss 1.7173 (1.9385)    Prec@1 57.422 (52.798)  Prec@5 83.594 (80.590)
Test: [70/196]  Time 0.516 (1.044)      Loss 1.3971 (1.8828)    Prec@1 64.453 (54.110)  Prec@5 87.500 (81.289)
Test: [80/196]  Time 0.765 (1.027)      Loss 2.1168 (1.8747)    Prec@1 55.078 (54.239)  Prec@5 78.125 (81.318)
Test: [90/196]  Time 1.136 (1.030)      Loss 2.4778 (1.8945)    Prec@1 41.016 (54.095)  Prec@5 72.656 (80.894)
Test: [100/196] Time 0.126 (1.006)      Loss 2.0996 (1.9239)    Prec@1 46.875 (53.697)  Prec@5 75.391 (80.411)
Test: [110/196] Time 1.061 (1.009)      Loss 1.5661 (1.9209)    Prec@1 63.672 (54.001)  Prec@5 83.984 (80.335)
Test: [120/196] Time 0.565 (1.001)      Loss 2.1030 (1.9204)    Prec@1 55.469 (54.358)  Prec@5 76.953 (80.220)
Test: [130/196] Time 2.475 (1.001)      Loss 1.2870 (1.9304)    Prec@1 70.703 (54.201)  Prec@5 87.891 (80.078)
Test: [140/196] Time 0.124 (0.987)      Loss 1.7190 (1.9237)    Prec@1 61.328 (54.446)  Prec@5 83.203 (80.156)
Test: [150/196] Time 2.323 (0.985)      Loss 1.7020 (1.9305)    Prec@1 64.062 (54.553)  Prec@5 80.078 (80.042)
Test: [160/196] Time 0.202 (0.975)      Loss 1.4141 (1.9326)    Prec@1 69.141 (54.612)  Prec@5 85.938 (80.049)
Test: [170/196] Time 2.498 (0.978)      Loss 1.1998 (1.9457)    Prec@1 69.922 (54.448)  Prec@5 92.188 (79.829)
Test: [180/196] Time 0.695 (0.967)      Loss 3.5546 (1.9594)    Prec@1 26.953 (54.299)  Prec@5 51.562 (79.588)
Test: [190/196] Time 2.084 (0.968)      Loss 2.2773 (2.0395)    Prec@1 46.094 (53.280)  Prec@5 78.516 (78.332)
 * Prec@1 53.136 Prec@5 78.124
```


