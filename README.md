# TransmogrifAI-ImageClassification

This repo has an image classification app built using [TransmogrifAI](https://github.com/salesforce/TransmogrifAI) AutoML capabilities.

### Dataset
Fashion MNIST from https://www.kaggle.com/zalando-research/fashionmnist/home is used for this app.

### AutoML Best Model Stats
```
"bestModelName" : "rfc_7003fd9e8d5f_2",
"cuttValues" : {
  "labelsKept" : [ 0.0, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0, 9.0 ],
  "labelsDropped" : [ ]
},
"trainingSetEvaluationResults" : {
  "(multiEval)_Error" : 0.09948177901725319,
  "(multiEval)_ThresholdMetrics" : {
    "topNs" : [ 1, 3 ],
    "noPredictionCounts" : {
      "1" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 2, 4, 5, 13, 20, 43, 61, 97, 127, 176, 237, 304, 392, 501, 611, 731, 865, 1031, 1234, 1454, 1673, 1917, 2220, 2506, 2816, 3176, 3572, 3965, 4374, 4821, 5257, 5729, 6187, 6638, 7110, 7557, 8012, 8458, 8904, 9382, 9866, 10348, 10832, 11267, 11705, 12204, 12690, 13107, 13571, 14053, 14581, 15065, 15546, 16061, 16599, 17072, 17588, 18142, 18714, 19275, 19856, 20431, 21059, 21652, 22278, 22860, 23458, 24058, 24765, 25472, 26255, 27087, 28048, 28956, 29924, 31000, 32199, 33668, 35612, 38680, 41353, 43963, 48049 ],
      "3" : [ 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 2, 4, 5, 13, 20, 43, 61, 97, 127, 176, 237, 304, 392, 501, 611, 731, 865, 1031, 1234, 1454, 1673, 1917, 2220, 2506, 2816, 3176, 3572, 3965, 4374, 4821, 5257, 5729, 6187, 6638, 7110, 7557, 8012, 8458, 8904, 9382, 9866, 10348, 10832, 11267, 11705, 12204, 12690, 13107, 13571, 14053, 14581, 15065, 15546, 16061, 16599, 17072, 17588, 18142, 18714, 19275, 19856, 20431, 21059, 21652, 22278, 22860, 23458, 24058, 24765, 25472, 26255, 27087, 28048, 28956, 29924, 31000, 32199, 33668, 35612, 38680, 41353, 43963, 48049 ]
    },
    "incorrectCounts" : {
      "1" : [ 4780, 4780, 4780, 4780, 4780, 4780, 4780, 4780, 4780, 4780, 4780, 4780, 4780, 4780, 4780, 4780, 4780, 4780, 4779, 4778, 4778, 4773, 4767, 4751, 4741, 4714, 4696, 4668, 4627, 4585, 4537, 4477, 4410, 4343, 4276, 4190, 4093, 3983, 3892, 3788, 3670, 3553, 3434, 3294, 3140, 3008, 2858, 2717, 2559, 2406, 2270, 2147, 1992, 1866, 1752, 1633, 1529, 1405, 1295, 1195, 1099, 1022, 943, 865, 784, 723, 671, 611, 549, 518, 470, 417, 380, 342, 310, 287, 258, 225, 203, 186, 164, 145, 134, 115, 98, 85, 76, 65, 58, 49, 41, 36, 32, 24, 17, 11, 4, 2, 0, 0, 0 ],
      "3" : [ 263, 264, 270, 281, 291, 303, 317, 338, 363, 390, 421, 454, 518, 575, 662, 764, 859, 970, 1088, 1237, 1362, 1502, 1667, 1812, 1955, 2094, 2231, 2339, 2460, 2582, 2691, 2784, 2892, 2956, 3043, 3115, 3169, 3191, 3234, 3246, 3260, 3237, 3211, 3132, 3034, 2942, 2819, 2703, 2556, 2406, 2270, 2147, 1992, 1866, 1752, 1633, 1529, 1405, 1295, 1195, 1099, 1022, 943, 865, 784, 723, 671, 611, 549, 518, 470, 417, 380, 342, 310, 287, 258, 225, 203, 186, 164, 145, 134, 115, 98, 85, 76, 65, 58, 49, 41, 36, 32, 24, 17, 11, 4, 2, 0, 0, 0 ]
    },
    "correctCounts" : {
      "1" : [ 43269, 43269, 43269, 43269, 43269, 43269, 43269, 43269, 43269, 43269, 43269, 43269, 43269, 43269, 43269, 43269, 43269, 43269, 43268, 43267, 43266, 43263, 43262, 43255, 43247, 43238, 43226, 43205, 43185, 43160, 43120, 43071, 43028, 42975, 42908, 42828, 42722, 42612, 42484, 42344, 42159, 41990, 41799, 41579, 41337, 41076, 40817, 40511, 40233, 39914, 39592, 39264, 38947, 38626, 38285, 37958, 37616, 37262, 36888, 36506, 36118, 35760, 35401, 34980, 34575, 34219, 33807, 33385, 32919, 32466, 32033, 31571, 31070, 30635, 30151, 29620, 29077, 28549, 27990, 27432, 26826, 26252, 25637, 25074, 24493, 23906, 23208, 22512, 21736, 20913, 19960, 19057, 18093, 17025, 15833, 14370, 12433, 9367, 6696, 4086, 0 ],
      "3" : [ 47786, 47785, 47779, 47768, 47758, 47746, 47732, 47711, 47686, 47659, 47628, 47595, 47531, 47474, 47387, 47285, 47190, 47079, 46959, 46808, 46682, 46534, 46362, 46194, 46033, 45858, 45691, 45534, 45352, 45163, 44966, 44764, 44546, 44362, 44141, 43903, 43646, 43404, 43142, 42886, 42569, 42306, 42022, 41741, 41443, 41142, 40856, 40525, 40236, 39914, 39592, 39264, 38947, 38626, 38285, 37958, 37616, 37262, 36888, 36506, 36118, 35760, 35401, 34980, 34575, 34219, 33807, 33385, 32919, 32466, 32033, 31571, 31070, 30635, 30151, 29620, 29077, 28549, 27990, 27432, 26826, 26252, 25637, 25074, 24493, 23906, 23208, 22512, 21736, 20913, 19960, 19057, 18093, 17025, 15833, 14370, 12433, 9367, 6696, 4086, 0 ]
    },
    "thresholds" : [ 0.0, 0.01, 0.02, 0.03, 0.04, 0.05, 0.06, 0.07, 0.08, 0.09, 0.1, 0.11, 0.12, 0.13, 0.14, 0.15, 0.16, 0.17, 0.18, 0.19, 0.2, 0.21, 0.22, 0.23, 0.24, 0.25, 0.26, 0.27, 0.28, 0.29, 0.3, 0.31, 0.32, 0.33, 0.34, 0.35, 0.36, 0.37, 0.38, 0.39, 0.4, 0.41, 0.42, 0.43, 0.44, 0.45, 0.46, 0.47, 0.48, 0.49, 0.5, 0.51, 0.52, 0.53, 0.54, 0.55, 0.56, 0.57, 0.58, 0.59, 0.6, 0.61, 0.62, 0.63, 0.64, 0.65, 0.66, 0.67, 0.68, 0.69, 0.7, 0.71, 0.72, 0.73, 0.74, 0.75, 0.76, 0.77, 0.78, 0.79, 0.8, 0.81, 0.82, 0.83, 0.84, 0.85, 0.86, 0.87, 0.88, 0.89, 0.9, 0.91, 0.92, 0.93, 0.94, 0.95, 0.96, 0.97, 0.98, 0.99, 1.0 ]
  },
  "(multiEval)_Precision" : 0.9017349192060385,
  "(multiEval)_F1" : 0.9011261593988766,
  "(multiEval)_Recall" : 0.9005182209827467
}
```