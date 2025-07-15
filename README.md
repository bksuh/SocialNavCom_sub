# SocialNavCom_sub
docker
```
docker run --rm -it \
    --gpus all \
    --runtime=nvidia \
    -v /home/bksuh/Desktop/SocialNavCom/SocialNavCom_sub:/app/Falcon/input:ro \
    -v /home/bksuh/Desktop/SocialNavCom/data:/app/Falcon/data:ro \
    zeyinggong/robosense_socialnav:v0.5
```
without read-only
```
docker run --rm -it \
    --gpus all \
    --runtime=nvidia \
    -v /home/bksuh/Desktop/SocialNavCom/SocialNavCom_sub:/app/Falcon/input \
    -v /home/bksuh/Desktop/SocialNavCom/data:/app/Falcon/data:ro \
    zeyinggong/robosense_socialnav:v0.5
```
without **rm**
```
docker run -it \
    --gpus all \
    --runtime=nvidia \
    -v /home/bksuh/Desktop/SocialNavCom/SocialNavCom_sub:/app/Falcon/input \
    -v /home/bksuh/Desktop/SocialNavCom/data:/app/Falcon/data:ro \
    zeyinggong/robosense_socialnav:v0.5
```
---
```
python -u -m habitat_baselines.eval --config-name=falcon_hm3d_replay.yaml
```

```
python -u -m habitat_baselines.eval --config-name=falcon_hm3d_val.yaml
```
