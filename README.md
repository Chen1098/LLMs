# Build your LLM step by step
1. Download Anaconda Prompt
2. in python testing mkdir fcc-gpt-course
3. in python testing python -m venv cuda
4. in python testing cuda\Scripts\activate
5. download visual studio build tools 2022 and start it
6. in python testing pip3 install matplotlib numpy pylzma ipykernel
7. in python testing pip3 install torch --index-url https://download.pytorch.org/whl/cu118
8. check python version 3.8~3.11 using python --version in python testing
9. in fcc-gpt-course type jupyter notebook
10. in fcc-gpt-course python -m ipykernel install --user --name=cuda --display-name "cuda-gpt"
11. type jupyter notebook in fcc-gpt-course
12. check the kernal section in jupyter notebook to see if cuda success
13. download large tar file with all the txt to learn from you can get the file free from https://skylion007.github.io/OpenWebTextCorpus/
14. in fcc-gpt-course\openwebtext run python data-extract.py
15. use data-extract.py to extract the smaller files from the large files don't forget to change the folder path
16. wait for a very very long time until it is done (1~2hours)
17. if eval loss is smaller than train loss it means that the neurons are nearly done 
18. pip3 install torch
19. run python chatbot.py -batch_size 32  to start the whole thing


1. play around with block size and batch size to try and fill gpu's memory (try not to use RAM)
block_size=input+max_new_tokens if the total size is greater than max_new_tokens than there will be an error so don't forget to increase block_size when input is very large
