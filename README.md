<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>


## Stack
  * Nest
  * MongoDB
  * Docker
mongodb

# Execute in development

1. Clone repository
2. Execute
```
 yarn install 
```` 
3.  Install Nest CLI
``` 
   npm i -g @nestjs/cli
```

4. Run mongodb
```
  docker-compose up -d
```

5. Copi file __.env.example__ and rename to __.env__

6. Fill variables in  __.env__

7. Run application 
```
  npm run:dev
```

8. Runn seed
```
  http://localhost:3000/api/v1/seed
```

# Production build
1.Crete file ```.env.prod```
2. Fill ```.env.prod``` variables
3. Build new image
   ```
   docker-compose -f docker-compose.prod.yaml --env-file .env.prod up --build
   ```