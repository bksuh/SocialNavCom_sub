# SocialNavCom_sub
docker commands
```
docker run --rm -it \
    --gpus all \
    --runtime=nvidia \
    -v /home/bksuh/Desktop/SocialNavCom/SocialNavCom_sub:/app/Falcon/input:ro \
    -v /home/bksuh/Desktop/data:/app/Falcon/data:ro \
    zeyinggong/robosense_socialnav:v0.5
```
