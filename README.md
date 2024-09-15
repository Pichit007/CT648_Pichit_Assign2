IP Address : http://175.41.173.29/

1. ทำการสร้าง Instance AWS
2. ทำการ Pull ไฟล์จาก Github มาบน AWS
3. ทำการ Create Dockerfile <br>

Dockerfile 
---------------------------------------
FROM oven/bun
COPY . .
RUN bun install
CMD ["bun","run","start"]
--------------------------------------- <br>

4. ทำการ Build Docker images
Build Docker images
---------------------------------------
sudo docker build -t pichit007/bunbasic:web .
--------------------------------------- <br>

5. ทำการ Run images Docker
---------------------------------------
sudo docker run -it -d -p 80:3000 pichit007/bunbasic:web
---------------------------------------
