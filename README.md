# Controle de Servo Motor com PWM no Raspberry Pi Pico W

## 📌 Descrição do Projeto
Este projeto implementa o **controle de um servomotor** utilizando **modulação PWM** no **Raspberry Pi Pico W**, seguindo as diretrizes da tarefa. A simulação foi realizada na plataforma **Wokwi**, com integração ao **Pico SDK** no VS Code.

## 🎥 Demonstração
O vídeo com a execução da simulação pode ser acessado em:
[🔗 Link para o vídeo](https://www.youtube.com/watch?v=8tvOLoBXICI&ab_channel=LorenzoGiuseppeOliveiraBaroni)

## 📜 Requisitos
- **Raspberry Pi Pico W**
- **Pico SDK instalado**
- **Simulador Wokwi**
- **Compilador ARM (arm-none-eabi-gcc)**
- **VS Code com extensão CMake**

## ⚙️ Configuração do PWM
- **Frequência:** 50 Hz (período de 20ms)
- **GPIO Utilizado:** 22
- **Ciclo de Trabalho para Controle do Servo:**
  - 2400µs → **Posição de 180 graus**
  - 1470µs → **Posição de 90 graus**
  - 500µs → **Posição de 0 graus**

## 📂 Estrutura do Código
O código segue os seguintes passos:
1. **Inicializa o PWM na GPIO 22**
2. **Movimenta o servo motor para posições pré-definidas** (0º, 90º e 180º)
3. **Implementa um movimento contínuo entre 0º e 180º** com incrementos suaves de **5µs**
4. **Integração com o LED RGB na GPIO 12**, observando variações no brilho

## 🔧 Como Compilar e Executar
### 1️⃣ Clonar o repositório
```bash
git clone https://github.com/lorenzobaroni/pwm_servo.git
```

### 2️⃣ Configurar o ambiente
Certifique-se de que o **Pico SDK** está configurado corretamente e que você tem o **CMake** instalado.


### 3️⃣ Executar no simulador Wokwi
Abra o **Wokwi** e carregue o código.

## 🎯 Observações sobre o LED RGB (BitDogLab)
Ao integrar o **LED RGB** na **GPIO 12**, foi observado que:
- O brilho do LED pode variar conforme a movimentação do servo.
- Se o servo exigir mais corrente, pode haver flutuações na alimentação do LED.

## 📌 Conclusão
Este projeto demonstrou com sucesso o **controle de um servomotor via PWM** utilizando o **Raspberry Pi Pico W**, além de integrar testes com um **LED RGB**. A implementação seguiu as diretrizes especificadas na tarefa, garantindo movimentação suave e precisão nas posições do servo.

---

## 📝 Licença
Este programa foi desenvolvido como um exemplo educacional e pode ser usado livremente para fins de estudo e aprendizado.

## 📌 Autor
LORENZO GIUSEPPE OLIVEIRA BARONI

