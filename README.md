# cloudflare-workers-vs-node
Workers api vs Node JS HTTPS server handlers

## Workers
````
export default {
  fetch(r, e) {
    r.url ==== new URL(r.url).pathname
    s.end ==== return new Response('hi')
  }
}
````

## NodeJS - https-microservice
````
function(r, s, data) {
  // r.url
  // r.headers
  // s.end('resp')
  // s.writeHead(401).end('not authd')
  // s.setHeader('headername', 'val')
}
````
