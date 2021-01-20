# Developpement de l'application mobile Daivery

20/01/2021 - mise en place d'un environnement de developpement d'appplication mobile. (principalement IOS pour l'instant)
- Installation de CocoaPods sur Windows ( Prérequis : Ruby, curl, git, CocoaPods) 
- Installation du Node.js / npm
- npm install react-native cli
- npm install --global expo-cli (expo client sur ios)
- pod install
- Création d'un repertoire (cd + npm install + npm init )
- cmd : expo start
- App.js ( Editeur actuel : Atom)

## Pour webview simple avec un site en ligne : App.js
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

> Note: En cours de rédaction ...



Si vous les trouvez utiles, n'oubliez pas de mettre une ⭐ et de la partager avec vos amis ❤️


Suivez moi sur [twitter](https://twitter.com/srfoj/)
