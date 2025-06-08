
# Projetos de Sistemas Embarcados - EmbarcaTech 2025

Autor: Antonio Carlos Ferreira de Almeida

Curso: Residência Tecnológica em Sistemas Embarcados

Instituição: EmbarcaTech - HBr

Campinas, 08 de junho de 2025

---

# 🎙️ BitDogLab Audio Recorder

Este projeto implementa um **gravador e reprodutor de áudio** usando a plataforma **BitDogLab (Raspberry Pi Pico)**, com linguagem **C estruturado**.

O sistema interage com o usuário através de **botões físicos**, fornece **feedback visual com LED RGB** e **exibe a forma de onda no display OLED** durante a reprodução.

## 📦 Funcionalidades

- 🎚️ **Gravação de áudio** por ADC (com taxa de amostragem ajustável)
- 🔊 **Reprodução de áudio** usando PWM
- 🎛️ **Controle por botões físicos**:
  - `BOTÃO RECORD`: inicia gravação
  - `BOTÃO PLAY`: reproduz o áudio
- 🌈 **Feedback visual** com LED RGB:
  - Vermelho: gravação
  - Verde: reprodução
  - Desligado: inativo
- 📺 **Visualização da forma de onda** gravada no display OLED

## 🧰 Componentes utilizados

- **BitDogLab (Raspberry Pi Pico W)**
- **ADC interno** do RP2040
- **Display OLED** da BDL com comunicação I2C
- **LED RGB** da BDL
- **Botões físicos (GPIO)** da BDL
- **PWM para saída de áudio** do RP2040
- **DMA** para leitura eficiente do ADC do RP2040

---

## 📜 Licença
GNU GPL-3.0.

