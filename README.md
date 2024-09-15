IP Address : http://175.41.173.29/

1. ทำการสร้าง Instance AWS
2. ทำการ Pull ไฟล์จาก Github มาบน AWS
3. ทำการ Create Dockerfile <br>

Dockerfile <br>
--------------------------------------- <br>
FROM oven/bun <br>
COPY . . <br>
RUN bun install <br>
CMD ["bun","run","start"] <br>
--------------------------------------- <br>

4. ทำการ Build Docker images <br>
Build Docker images <br>
--------------------------------------- <br>
sudo docker build -t pichit007/bunbasic:web . <br>
--------------------------------------- <br>

5. ทำการ Run images Docker <br>
--------------------------------------- <br>
sudo docker run -it -d -p 80:3000 pichit007/bunbasic:web <br>
--------------------------------------- <br>
