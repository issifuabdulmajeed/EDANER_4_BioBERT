Run the following.

1. Preprocess data :
    cd named-entity-recognition
    ./preprocess.sh
2.
python run_ner.py --data_dir ../datasets/NER/AUG-NCBI-disease --labels ../datasets/NER/AUG-NCBI-disease/labels.txt -
-model_name_or_path dmis-lab/biobert-base-cased-v1.1 --output_dir output/AUG-NCBI-disease --max_seq_length 128 --num_train_epochs 3 --per_device_train_batch_size 32 --save_steps 1000 --seed 1--do_train --do_eval --do_predict --overwrite_output_dir
