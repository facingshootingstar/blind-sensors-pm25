# Blind Sensors: Transferring Satellite-Informed PM2.5 Models to Cities Without Monitors

## Abstract
Air-quality ML is usually validated where monitors exist. We measure the gap between in-distribution performance and leave-city-out transfer using satellite-like AOD and meteorology features—simulating cities that lack ground sensors.

## Results (notebook run)
Leave-city-out MAE by city:
```
     city       mae      auc
    Hanoi 13.022945 0.979751
      HCM  7.546792 0.964257
  Bangkok  9.986797 0.975833
  Jakarta 10.179929 0.965901
   Manila  6.304216 0.978306
Singapore 13.088171 0.976846
ChiangMai  5.665289 0.979962
   CanTho  5.406550 0.978214
```

## Conclusion
Large LCO degradation means satellite features alone do not close the sensor gap; equity analyses must report transfer, not pooled CV.

## Code
`notebook/blind-sensors-pm25-transfer.ipynb` — independent repository.
