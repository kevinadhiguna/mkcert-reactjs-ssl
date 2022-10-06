# Mkcert ReactJS - SSL 🔒

a React app using HTTPS for Local Development powered by [mkcert](https://github.com/FiloSottile/mkcert).

<img src="https://i.ibb.co/z2pc6FH/react-app-HTTPS.png" />

<br />

## How to Run

1) Clone this repo :
```
git clone https://github.com/kevinadhiguna/mkcert-reactjs-ssl.git
```

<br />

2) Open Terminal and change directory to mkcert-reactjs-ssl :
```
cd mkcert-reactjs-ssl
```

<br />

3) Install dependencies :
```
yarn
```

or

```
yarn install
```

Note: with npm, it would be :
```
npm install
```

<br />

4) Run the React app :
```
yarn devStart
```

Note: with npm, it would be
```
npm run devStart
```

Runs the app in the development mode with HTTPS.\
Open [https://localhost:3000](https://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

<br />

## Configuring HTTPS

Go to `package.json` and change the script to :

### Windows
```json
"scripts": {
  "devStart":
    "set HTTPS=true&&set SSL_CRT_FILE={CERT-PATH}&&set SSL_KEY_FILE={KEY-PATH}&&react-scripts start"
}
```

<br />

### Linux & MacOS
```json
"scripts": {
  "devSstart":
    "HTTPS=true SSL_CRT_FILE={CERT-PATH} SSL_KEY_FILE={KEY-PATH} react-scripts start"
}
```

Please replace `{CERT-PATH}` and `{KEY-PATH}` to yours. It will be generated after `mkcert localhost` command.

<br />

## Acknowledgement
- [mkcert](https://github.com/FiloSottile/mkcert)
- [Bits and Pieces - Using HTTPS for Local Development for React, Angular, and Node](https://blog.bitsrc.io/using-https-for-local-development-for-react-angular-and-node-fdfaf69693cd)

<br />

![Hello !](https://api.visitorbadge.io/api/VisitorHit?user=kevinadhiguna&repo=mkcert-reactjs-ssl&label=thanks%20for%20dropping%20in%20!&labelColor=%23000000&countColor=%23FFFFFF)
