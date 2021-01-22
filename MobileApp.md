# Developpement de l'application mobile Daivery
Utilisation du framework [react-native de Facebook](https://reactnative.dev/)<br>
20/01/2021 - mise en place d'un environnement de développement d'application mobile. (principalement IOS pour l'instant)
- Installation de CocoaPods sur Windows ( Prérequis : Ruby, curl, git, CocoaPods) 
- Installation du Node.js / npm
- npm install react-native cli
- npm install --global expo-cli (expo client sur ios)
- pod install
- Création d'un répertoire (cd + npm install + npm init )
- cmd : expo start
- App.js ( Editeur actuel : Atom)

## Pour une webview simple avec un site en ligne : App.js
```jsx

import { StatusBar } from 'expo-status-bar';
import React from 'react';
import { StyleSheet, Text, View } from 'react-native';
import { WebView } from 'react-native-webview';
import { AppLoading } from 'expo';
import { SafeAreaView } from 'react-native-safe-area-context';



export default function App() {
  return (
    <WebView
      originWhitelist={['*']}
      source={{
          uri: 'https://daivery.com'
        }}
    />
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#fff',
    alignItems: 'center',
    justifyContent: 'center',
  },
});

```


## Documentation

> Notes: En cours de rédaction ...



Si vous trouvez utile ce readme, n'oubliez pas de mettre une ⭐ et de le partager avec vos amis ❤️


Suivez-moi sur [twitter](https://twitter.com/srfoj/)
