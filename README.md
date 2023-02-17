<p align="center">
  <img src = "https://user-images.githubusercontent.com/60518209/219722904-99aece3e-6ffa-48be-8cdc-0cc4e83ad4e4.png" width = "630" />
  <img src = "https://user-images.githubusercontent.com/60518209/219722908-b4e7ec81-d205-430b-b1b6-7575e96da3a9.png" width = "630" />
</p>

# Prediction_SDRS
Prediction of secondary dendrite arm spacing in Al alloys using machine learning

## Abstract
In this study, three machine learning (ML) models were developed to predict the secondary dendrite arm spacing (SDAS) and then predictions were validated experimentally. First, a three-layer artificial neural networks (ANN) was built to predict the SDAS. Then, a linear regression model (LR) with backward selection method is applied to study the relationship of different elemental properties, processing parameters, and SDAS and make a prediction. A principle component analysis (PCA) further explores these relationships. The results show that the ANN model has the best performance compared with the LR and PCA models. Compared with the classical coarsening equation, the current SDAS predictions reveal a deviation from nearly linear relationship with the negative cubic root of cooling rate, which indicates there are other elemental properties that should be accounted for.

## Background
During the casting process of Al alloys, the cast part commonly solidifies with a dendritic structure. The dendrites consist of primary, secondary and sometimes tertiary dendrite arms. The dendritic structure has an important property, namely that the SDAS increases during solidification and thus the microstructure coarsens. The characteristic geometric property of dendrites is that the secondary dendrite arm spacing (SDAS) becomes larger during solidification. It can take place in such a way that the thicker and longer arms continue to grow, while the smaller ones shrink and dissolve. This is due to the concentration difference at the surface as well as different radii of curvature. When a smaller arm disappears entirely, the distance between the neighboring arms becomes larger. The driving force for this process is the reduction of the solid/liquid interface energy .For a larger wall thickness aluminum casting, the SDAS can negatively influence its properties to a greater extent (e.g. tensile strength, deformability, etc.). However, one of the critical issue in the cast aluminum alloy is how to effectively and efficiently predict the SDAS size. Although the effect of concentration, solidification parameters (especially cooling rate and local solidification time) influencing the SDAS has been studied by experiments and as a result, analytical and numerical models have been developed to describe the coarsening phenomenon, accurately computing the SDAS using these parameters is impractical for these multi-component alloys over wide ranges of temperatures and compositions in a high throughput manner. Therefore, to rationalize this problem, a number of empirical or semi-empirical rules were proposed, which were mainly based on whether there was a correlation between the SDAS and several empirical parameters that could be calculated readily from the Al alloy composition, such as the mixing entropy $a_{\Delta S_{mix}}$, the parameters of atomic size difference $s_{R}$ and the average mixing enthalpy $a_{H}$, the mean valance electron concentration $a_{VEC}$ and the electronegativity parameters $a_{PE}$, the average specific heat capacity of mixing $a_{C}$, the average thermal expansion of mixing $a_{a}$ and many others.\\
ANN is a powerful algorithm that could handle complex problem not only in the computer science field, such as computer vision and natural language processing , but also in the materials informatics. Comparing to the other powerful algorithms, the ML process based on the ANN algorithm is much easier to be interpreted, which could help us to better understand the influence of different features on the results and to explore the underlying physical mechanism. In this study, three ML models, namely ANN, LR and PCA were built to predict SDAS with the consideration of elemental properties, and then they were experimentally validated to ensure their accuracy. Cross-validation was applied to evaluate the performance of the ML models. Correlation of different elemental properties with SDAS is explored. After the models were built, the SDAS of Al-4.5\%Cu and A356 alloy under different processing conditions were predicted and compared against experimental results. Furthermore, a conclusion was drawn based on the SDAS data and the developed models. This conclusion is different from that developed from the  coarsening equation, which predicts a linear relationship between SDAS and negative cubic root of cooling rate. Thus, there are other factors also playing an important role in determining the SDAS.
