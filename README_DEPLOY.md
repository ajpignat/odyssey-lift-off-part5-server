change ./src/index.js
from
const { url, port } = await server.listen();
to
const { url, port } = await server.listen({ port: process.env.PORT || 4000 });
