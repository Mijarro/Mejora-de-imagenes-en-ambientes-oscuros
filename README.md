# **Visión Artificial - UNIR**  
# **Actividad 1: Mejora de imagen con operaciones elementales.**

### **Autor:** Miguel Jara Arroyo

Este proyecto aborda la mejora de imágenes capturadas en condiciones de baja iluminación utilizando el conjunto de datos **The Dark Face**. Se implementaron y compararon dos métodos principales de ajuste de iluminación: uno por canal y otro global, evaluando sus ventajas y limitaciones.

---

### **Documentación**  
Puedes consultar la documentación completa en formato PDF en el siguiente enlace:  
[Actividad_1_UNIR_VA.pdf](https://github.com/Mijarro/Mejora-de-imagenes-en-ambientes-oscuros/blob/main/Actividad_1_UNIR_VA.pdf)

---

## **Metodología**

1. **Análisis inicial**:  
   - Se analizaron histogramas de intensidad RGB para identificar características de las imágenes.  
   - Los valores de intensidad se encuentran principalmente entre 0 y 50, con excepciones en imágenes con luz artificial.  

2. **Ajuste inicial**:  
   - Multiplicación de la intensidad de los píxeles por un factor constante (\(f = 2.5\)).  
   - Resultados: Mejora en áreas oscuras, pero con "quemado" en zonas bien iluminadas.  

3. **Ajustes dinámicos**:  
   - **Por canal**: Factor calculado individualmente para cada canal RGB.  
   - **Global**: Factor basado en el brillo promedio de toda la imagen.  
   - Ambos métodos ajustan el brillo según una iluminación objetivo predeterminada.  

---

## **Resultados**

- **Ajuste por canal**:  
  - Mejora significativa en áreas oscuras y definición.  
  - Introduce distorsión cromática, con predominio del azul en imágenes muy oscuras.  

  ![image](https://github.com/user-attachments/assets/1f630795-6d83-48b2-b7bc-7d2e23733c56)

- **Ajuste global**:  
  - Genera imágenes más naturales y con mejor balance cromático.  
  - Ligera pérdida de detalle en áreas muy oscuras en comparación con el ajuste por canal.  

  ![image](https://github.com/user-attachments/assets/11983edf-e6e7-4de0-ba22-8daf3e74fc2a)

---

## **Conclusiones**

1. **Ajuste por canal**: Adecuado para aplicaciones computacionales donde la precisión de detalles es clave.  
2. **Ajuste global**: Mejor para visualización por usuarios humanos, priorizando el balance tonal y la naturalidad.  

Ambos métodos tienen fortalezas específicas, pero podrían combinarse en modelos híbridos para aprovechar sus ventajas. El desarrollo de algoritmos no lineales es una dirección prometedora para superar las limitaciones actuales y mejorar la calidad del procesamiento de imágenes en condiciones de iluminación difíciles.

---

## **Referencia al conjunto de datos**  

Yang, Wenhan, Yuan, Ye, Ren, Wenqi, Liu, Jiaying, Scheirer, Walter J., Wang, Zhangyang, Zhang, and et al. (2020).  
*Advancing Image Understanding in Poor Visibility Environments: A Collective Benchmark Study.*  
IEEE Transactions on Image Processing, 29, 5737-5752.  
DOI: [10.1109/TIP.2020.2981922](https://doi.org/10.1109/TIP.2020.2981922)  

---
---

# English:
# **Computer Vision - UNIR**  
# **Activity 1: Image Enhancement with Basic Operations**

### **Author:** Miguel Jara Arroyo

This project focuses on enhancing images captured under low-light conditions using the **The Dark Face** dataset. Two main illumination adjustment methods were implemented and compared: a per-channel method and a global method, evaluating their advantages and limitations.

---

### **Documentation**  
You can find the full documentation in PDF format at the following link:  
[Actividad_1_UNIR_VA.pdf](https://github.com/Mijarro/Mejora-de-imagenes-en-ambientes-oscuros/blob/main/Actividad_1_UNIR_VA.pdf)

---

## **Methodology**

1. **Initial Analysis**:  
   - RGB intensity histograms were analyzed to identify image characteristics.  
   - Intensity values are mainly between 0 and 50, with exceptions in images with artificial light.  

2. **Initial Adjustment**:  
   - Pixel intensity was multiplied by a constant factor (\(f = 2.5\)).  
   - Results: Improved dark areas but introduced "burning" in well-lit regions.  

3. **Dynamic Adjustments**:  
   - **Per-Channel**: Factor calculated individually for each RGB channel.  
   - **Global**: Factor calculated based on the average brightness of the entire image.  
   - Both methods adjust brightness to meet a predefined target illumination level.  

---

## **Results**

- **Per-Channel Adjustment**:  
  - Significant improvement in dark areas and better definition.  
  - Introduced chromatic distortion, with a blue shift in very dark images.  

  ![image](https://github.com/user-attachments/assets/1f630795-6d83-48b2-b7bc-7d2e23733c56)

- **Global Adjustment**:  
  - Produced more natural images with better color balance.  
  - Slight loss of detail in very dark areas compared to the per-channel adjustment.  

  ![image](https://github.com/user-attachments/assets/11983edf-e6e7-4de0-ba22-8daf3e74fc2a)

---

## **Conclusions**

1. **Per-Channel Adjustment**: Suitable for computational applications where detail precision is critical.  
2. **Global Adjustment**: Better suited for human viewing, prioritizing tonal balance and naturalness.  

Both methods have specific strengths, but combining them into hybrid models could leverage their advantages. Developing non-linear algorithms is a promising direction to overcome current limitations and improve the quality of image processing under challenging lighting conditions.

---

## **Dataset Citation**  

Yang, Wenhan, Yuan, Ye, Ren, Wenqi, Liu, Jiaying, Scheirer, Walter J., Wang, Zhangyang, Zhang, and et al. (2020).  
*Advancing Image Understanding in Poor Visibility Environments: A Collective Benchmark Study.*  
IEEE Transactions on Image Processing, 29, 5737-5752.  
DOI: [10.1109/TIP.2020.2981922](https://doi.org/10.1109/TIP.2020.2981922)  

