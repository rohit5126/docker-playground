# Pin a specific Node version (never a floating `latest`).
FROM node:20-alpine AS prod

WORKDIR /app


# Copy the source and build the production bundle into /dist.
COPY . .

RUN npm install && npm run build


RUN addgroup -S app && adduser -S -G app app
RUN chown -R app:app /app
USER app

# Vite preview serves the built bundle on this port.
EXPOSE 4173

# 0.0.0.0 so the server is reachable from outside the container.
CMD ["npm", "run", "preview", "--", "--host", "0.0.0.0", "--port", "4173"]
