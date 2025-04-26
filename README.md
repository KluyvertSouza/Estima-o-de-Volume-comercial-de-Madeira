# Estimação de Volume comercial de Madeira
O trabalho visa desenvolver equação de volume comercial de várias espécies, feita com a cubagem rigorosa baseado no romaneio de toras da concessão florestal da Floresta Nacional de Altamira-PA. Além de oferecer aos órgãos ambientais, empresas e produtores do setor florestal praticidade e maior precisão volumétrica nos planos de manejo florestal.

Essa rotina pode ser aplicada para todos os modelos e unidades de manejo florestal da base de dados. A espécie mais frequênte foi a *Tabebuia serratifolia*, o grupo mais frequente foi o ALT3_UPA2, que se refere ao espaço cedido para manejo florestal, onde o dado foi coletado, então será usado como exemplo. Os grupos causam diferença principalmente entre a idade das árvores, por tanto, não separar por grupo pode gerar heterocedasticidade dos resíduos.

Separado os dados, podemos fazer treinar diferentes modelos para predição, já que o propósito é avaliar qual modelo é mais apropriado.

| Modelo | Relação matemática (modelos) | Autores             |
|--------|--------------------------------|---------------------|
| 1      | $v = \beta_0 + \beta_1 d + \varepsilon_i$ | Berkhant            |
| 2      | $v = \beta_0 + \beta_1 d^2 + \varepsilon_i$ | Koperzky e Gehrhardt |
| 3      | $v = \beta_0 + \beta_1 d + \beta_2 d^2 + \varepsilon_i$ | Hohenadl e Krenn    |
| 4      | $\log v = \beta_0 + \beta_1 \log d + \beta_2 \frac{1}{d} + \varepsilon_i$ | Brenac              |
| 5      | $\log v = \beta_0 + \beta_1 \log d + \varepsilon_i$ | Husch


Note que, para a criação de predição em si, nenhum pressuposto foi estabelecido.
