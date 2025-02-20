# AR React Native Jorge

Este repositorio contiene una aplicación React Native para AR (Realidad Aumentada). A continuación se detallan los pasos para configurar y ejecutar la aplicación en tu entorno local.

## Requisitos previos

Antes de comenzar, asegúrate de tener instalados los siguientes componentes en tu máquina:

- **Node.js**: [Descargar Node.js](https://nodejs.org/)
- **npm o yarn**: npm se instala automáticamente con Node.js, pero puedes usar [Yarn](https://yarnpkg.com/) si prefieres.
- **React Native CLI** (si usas React Native CLI en vez de Expo):
  ```bash
  npm install -g react-native-cli
  ```
- **Android Studio o Xcode** (para Android o iOS respectivamente).

Para instalar Android Studio y Xcode para dispositivos iOS, sigue la documentación oficial de React Native para configurar tu entorno de desarrollo.

## Instalación

Sigue los siguientes pasos para instalar y ejecutar la aplicación en tu máquina.

### 1. Clonar el repositorio

Primero, clona el repositorio a tu máquina local:

```bash
git clone https://github.com/Jorgesannchezz/AR_React_Native_Jorge.git
```

### 2. Navegar al directorio del proyecto

Accede al directorio del proyecto:

```bash
cd AR_React_Native_Jorge
```

### 3. Instalar dependencias

Instala las dependencias necesarias utilizando npm o yarn. Si usas npm, ejecuta:

```bash
npm install
```

Si prefieres yarn, ejecuta:

```bash
yarn install
```

### 4. Configurar entorno de desarrollo

#### Para Android:

- **Instalar Android Studio**: Asegúrate de tener Android Studio instalado y configurado. Esto incluye tener el emulador de Android configurado y las dependencias de SDK necesarias.
- **Configurar variables de entorno**: Asegúrate de que las variables de entorno de Android estén correctamente configuradas en tu sistema. Esto se puede hacer agregando lo siguiente en tu archivo `~/.bash_profile` o `~/.zshrc` (dependiendo de tu terminal):

```bash
export ANDROID_HOME=$HOME/Library/Android/sdk
export PATH=$PATH:$ANDROID_HOME/tools:$ANDROID_HOME/platform-tools
```

- **Ejecutar en un dispositivo/emulador Android**:

Si todo está configurado correctamente, puedes ejecutar el siguiente comando para lanzar la aplicación en un emulador o dispositivo conectado:

```bash
npx react-native run-android
```

#### Para iOS:

- **Instalar Xcode**: Asegúrate de tener Xcode instalado en tu máquina.
- **Instalar dependencias de iOS**: Si estás usando iOS, ejecuta este comando para instalar las dependencias de CocoaPods:

```bash
cd ios
pod install
cd ..
```

- **Ejecutar en un dispositivo/emulador iOS**:

Si todo está configurado correctamente, puedes ejecutar el siguiente comando para lanzar la aplicación en el emulador de iOS:

```bash
npx react-native run-ios
```

## Solución de problemas

Si experimentas problemas con las dependencias, intenta borrar la caché de npm/yarn y vuelve a instalar:

```bash
npm cache clean --force
npm install
```

O si usas yarn:

```bash
yarn cache clean
yarn install
```

Si tienes problemas con la ejecución en Android, asegúrate de tener el emulador correctamente configurado o de que un dispositivo Android esté conectado.
