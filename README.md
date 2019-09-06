# egg_detection

to run csv file:
normally run the file


TO run tf_record:
generate_tfrecord.py --csv_input=generate_tfrecord.py --csv_input="C:/Users/T Poornima/PycharmProjects/egg_detection/images/train_labels.csv" --image_dir="C:/Users/T Poornima/PycharmProjects/egg_detection/images/train" --output_path=train.record
Run again and replace train with test

train.py:
python train.py --logtostderr --train_dir="C:/Users/T Poornima/PycharmProjects/object_detection/training/"  --pipeline_config_path="C:/Users/T Poornima/PycharmProjects/object_detection/training/faster_rcnn_inception_v2_pets.config"


inference_graph:
export_inference_graph.py --input_type image_tensor --pipeline_config_path training/faster_rcnn_inception_v2_pets.config --trained_checkpoint_prefix training/model.ckpt-1096 --output_directory inference_graph

see the link and follow the remaining steps


