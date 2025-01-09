# slidev
https://cn.sli.dev/

```code
docker run --name slidev --rm -it \
    --user node \
    -v ${PWD}:/slidev \
    -p 3030:3030 \
    -e NPM_MIRROR="https://registry.npmmirror.com" \
    tangramor/slidev:latest

docker exec -it slidev \
       npx slidev build *.md \
                  -o abc \
                  --base ./ --download true
```


