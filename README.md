# Rock Paper Scissors (Jokenpo) — Jogo Android

![License](https://img.shields.io/badge/license-MIT-green)
![Platform](https://img.shields.io/badge/platform-Android-brightgreen)
![Language](https://img.shields.io/badge/language-Java-orange)
![Build](https://img.shields.io/badge/build-Gradle-blue)
![Min SDK](https://img.shields.io/badge/min%20SDK-21%2B-green)

Jogo clássico **Pedra, Papel e Tesoura (Jokenpo)** para Android, desenvolvido como exercício de aprendizado em desenvolvimento mobile nativo.

## 🎮 Sobre o Jogo

Implementação do tradicional jogo de mão onde:
- **Pedra** vence **Tesoura** (quebra)
- **Tesoura** vence **Papel** (corta)
- **Papel** vence **Pedra** (embrulha)

### Regras da Partida
- Escolha entre **Pedra 🪨**, **Papel 📄** ou **Tesoura ✂️**
- O computador faz sua escolha aleatoriamente
- **Melhor de 3 rodadas** — quem ganhar 2 vence a partida
- Sistema de **pontuação acumulada**
- **Cosméticos desbloqueáveis** com pontos ganhos

## 🎨 Design

![Design do Jogo](https://github.com/paulorabelo/rock-paper-scissors/blob/main/design.png)

*Interface intuitiva com Material Design, animações suaves e feedback visual.*

## 🛠️ Tecnologias

| Tecnologia | Versão/Uso |
|------------|------------|
| **Java** | 8+ (Linguagem principal) |
| **Android SDK** | API 21+ (Android 5.0 Lollipop+) |
| **Android Studio** | IDE oficial (Arctic Fox+) |
| **Gradle** | Build system (Groovy/Kotlin DSL) |
| **XML** | Layouts de UI |
| **Material Components** | Componentes visuais modernos |

## 🚀 Como Executar

### Pré-requisitos
- Android Studio instalado
- JDK 8 ou superior
- Dispositivo Android (API 21+) ou Emulador configurado

### Passos
```bash
# 1. Clone o repositório
git clone https://github.com/paulorabelo/rock-paper-scissors.git

# 2. Abra no Android Studio
# File > Open > Selecione a pasta do projeto

# 3. Aguarde sincronização do Gradle

# 4. Execute (Shift+F10 ou ▶️ Run)
#    - Emulador: crie um AVD no Device Manager
#    - Dispositivo físico: ative "Depuração USB" nas Opções do Desenvolvedor
```

## 📁 Estrutura do Projeto

```
rock-paper-scissors/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/example/rockpaperscissors/
│   │   │   │   ├── MainActivity.java       # Lógica principal do jogo
│   │   │   │   ├── GameLogic.java          # Regras e pontuação
│   │   │   │   └── CosmeticsManager.java   # Sistema de cosméticos
│   │   │   ├── res/
│   │   │   │   ├── layout/
│   │   │   │   │   ├── activity_main.xml   # Tela principal
│   │   │   │   │   └── item_cosmetic.xml   # Item de cosmético
│   │   │   │   ├── drawable/               # Ícones, backgrounds
│   │   │   │   ├── values/
│   │   │   │   │   ├── strings.xml
│   │   │   │   │   ├── colors.xml
│   │   │   │   │   └── themes.xml
│   │   │   │   └── anim/                   # Animações
│   │   │   └── AndroidManifest.xml
│   │   └── test/                           # Testes unitários
│   ├── build.gradle
│   └── proguard-rules.pro
├── build.gradle
├── settings.gradle
├── gradle.properties
├── gradlew / gradlew.bat                   # Gradle Wrapper
└── design.png                              # Mockup do design
```

## 🎯 Funcionalidades Implementadas

- [x] Lógica completa do jogo (Pedra/Papel/Tesoura)
- [x] Melhor de 3 rodadas
- [x] Pontuação persistente (SharedPreferences)
- [x] Sistema de cosméticos desbloqueáveis
- [x] Animações de transição entre rodadas
- [x] Feedback visual/vibratório
- [x] Tema Material Design responsivo
- [ ] Multiplayer local (Bluetooth/WiFi Direct) — *futuro*
- [ ] Ranking online (Firebase) — *futuro*
- [ ] Modo torneio — *futuro*

## 🧠 Conceitos Aprendidos

Este projeto serviu para praticar:
- **Activity Lifecycle** (onCreate, onStart, onResume, onPause, onStop, onDestroy)
- **ViewBinding** / findViewById para acesso a views
- **SharedPreferences** para persistência simples
- **Handler/Runnable** para delays e animações temporizadas
- **Random** para IA do computador
- **RecyclerView** para lista de cosméticos
- **Material Design Components** (Buttons, Cards, Dialogs)
- **Gradle** configuração e dependências

## 🤝 Contribuindo

Contribuições são bem-vindas! Ideias para melhorias:

1. Fork o projeto
2. Crie sua branch (`git checkout -b feature/nova-funcionalidade`)
3. Commit suas mudanças (`git commit -m 'feat: descrição'`)
4. Push (`git push origin feature/nova-funcionalidade`)
5. Abra um Pull Request

### Sugestões de contribuição
- Novos cosméticos/temas
- Melhorias na IA do computador
- Testes unitários (JUnit, Espresso)
- Acessibilidade (TalkBack, contrastes)
- Internacionalização (i18n)

## 📄 Licença

Este projeto está sob a licença **MIT**. Veja o arquivo [LICENSE](LICENSE) para detalhes.

## 👨‍💻 Autor

**Paulo Rabelo**
- GitHub: [@paulorabelo](https://github.com/paulorabelo)
- Blog: [blog.paulorabelo.dev.com.br](https://blog.paulorabelo.dev.com.br)
- LinkedIn: [Paulo Rabelo](https://www.linkedin.com/in/paulorabelooficial/)

---

*Desenvolvido como exercício de aprendizado em desenvolvimento Android nativo com Java. Cada linha de código representa um passo na jornada mobile! 🚀*
