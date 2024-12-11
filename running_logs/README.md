
```bash
(clinical_multimodal) ubuntu@ip-10-0-15-201:~/workspace/MAGIC/utils$ python trace_parser.py 
reading ta1-trace-e3-official-1.json.5 ...
5000000it [00:09, 532723.23it/s]
reading ta1-trace-e3-official-1.json.6 ...
2130374it [00:04, 507088.35it/s]
reading ta1-trace-e3-official-1.json.tar.gz ...
0it [00:00, ?it/s]
Traceback (most recent call last):
  File "/home/ubuntu/workspace/MAGIC/utils/trace_parser.py", line 246, in <module>
    read_graphs(args.dataset)
  File "/home/ubuntu/workspace/MAGIC/utils/trace_parser.py", line 191, in read_graphs
    preprocess_dataset(dataset)
  File "/home/ubuntu/workspace/MAGIC/utils/trace_parser.py", line 110, in preprocess_dataset
    for line in tqdm(f):
  File "/home/ubuntu/miniconda3/envs/clinical_multimodal/lib/python3.9/site-packages/tqdm/std.py", line 1181, in __iter__
    for obj in iterable:
  File "/home/ubuntu/miniconda3/envs/clinical_multimodal/lib/python3.9/codecs.py", line 322, in decode
    (result, consumed) = self._buffer_decode(data, self.errors, final)
UnicodeDecodeError: 'utf-8' codec can't decode byte 0x8b in position 1: invalid start byte
```