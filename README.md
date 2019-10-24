conda install pytorch=1.2.0 -c pytorch

*NO ESPECIFICAR TOOLKIT,el que ya tiene el servidor sirve*

bash init.sh (si sale error instalar lo que haga falta)

bash init_coco.sh (descarga y organiza automaticamente lo necesario *train,val y anotaciones*)

CUDA_VISIBLE_DEVICES=1 python -W ignore  upsnet/upsnet_end2end_train.py --cfg upsnet/experiments/upsnet_resnet50_coco_1gpu.yaml

-W ignore para que no saque molestos avisos de deprecacion
