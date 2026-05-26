# Disseny d'un model predictiu per a l'avaluació de la salut mental en entorns digitals de joc

Aquest repositori conté el codi font, els experiments i el pipeline de ciència de dades desenvolupats per al Treball Final de Màster (TFM) del Màster Universitari en Ciència de Dades de la Universitat Oberta de Catalunya (UOC).

## Descripció del Projecte
L'objectiu principal d'aquest treball és dissenyar, implementar i validar un model predictiu basat en aprenentatge automàtic (Machine Learning) i aprenentatge profund (Deep Learning) per identificar perfils de risc de salut mental (com ara addicció, ansietat o depressió) en jugadors de videojocs. 

Mitjançant l'anàlisi de patrons de comportament, hàbits de vida i nivells d'implicació financera, el model busca actuar com una prova de concepte metodològica per fomentar un disseny de videojocs més ètic i un consum digital saludable.

## Metodologia i Estructura del Codi
El projecte s'ha estructurat seguint el cicle de vida de la ciència de dades **CRISP-DM** i està dividit de forma modular en els següents blocs de desenvolupament (corresponents als Annexos de la memòria):

1. **Càrrega i Optimització del Dataset:** Tècniques de downcasting (`float32` i `category`) per gestionar eficientment un volum d'1 milió de registres en entorns de memòria RAM limitada.
2. **Anàlisi Exploratori de Dades (EDA):** Investigació de factors demogràfics, correlacions i detecció de valors anòmals.
3. **Preparació de Dades i Equilibri de Classes:** Implementació de l'algorisme SMOTE per resoldre el desbalanceig de la variable objectiu.
4. **Modelatge Baseline i Avançat:** Entrenament, optimització d'hiperparàmetres i avaluació de models combinatoris com *Random Forest* i *XGBoost*.
5. **Arquitectures Deep Learning:** Implementació del model *TabNet* (Tabular Attentive Network) adaptat a dades tabulars de gran escala.
6. **Intel·ligència Artificial Explicable (XAI):** Aplicació de mètodes d'interpretabilitat per identificar les variables d'impacte en el benestar de l'usuari.

## Tecnologies Utilitzades
* **Llenguatge:** Python 3
* **Llibreries principals:** Pandas, NumPy, Scikit-Learn, XGBoost, PyTorch-TabNet, Imbalanced-Learn, Matplotlib, Seaborn.
* **Entorn:** Google Colab / Jupyter Notebooks.
