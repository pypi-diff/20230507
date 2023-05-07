# Comparing `tmp/haloop-0.0.6.tar.gz` & `tmp/haloop-0.0.7.tar.gz`

## Comparing `haloop-0.0.6.tar` & `haloop-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 haloop-0.0.6/.github/workflows/release.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/__init__.py
--rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/beam.py
--rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/ctc.py
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/data.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/loop.py
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/model.py
--rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/resnet.py
--rw-r--r--   0        0        0    13671 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/rnnlm.py
--rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/scan.py
--rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/star.py
--rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/symbol_tape.py
--rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/transducer.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 haloop-0.0.6/ha/xen.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 haloop-0.0.6/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 haloop-0.0.6/LICENSE
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 haloop-0.0.6/README.md
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 haloop-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 haloop-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 haloop-0.0.7/.github/workflows/release.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/__init__.py
+-rw-r--r--   0        0        0    10031 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/attention.py
+-rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/beam.py
+-rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/ctc.py
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/data.py
+-rw-r--r--   0        0        0    14041 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/loop.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/model.py
+-rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/resnet.py
+-rw-r--r--   0        0        0    13671 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/rnnlm.py
+-rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/scan.py
+-rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/star.py
+-rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/symbol_tape.py
+-rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/transducer.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 haloop-0.0.7/ha/xen.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 haloop-0.0.7/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 haloop-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 haloop-0.0.7/README.md
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 haloop-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 haloop-0.0.7/PKG-INFO
```

### Comparing `haloop-0.0.6/.github/workflows/release.yml` & `haloop-0.0.7/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `haloop-0.0.6/ha/beam.py` & `haloop-0.0.7/ha/beam.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.6/ha/ctc.py` & `haloop-0.0.7/ha/ctc.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.6/ha/data.py` & `haloop-0.0.7/ha/data.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.6/ha/loop.py` & `haloop-0.0.7/ha/loop.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 
 from .data import concat_datasets
 from .beam import ctc_beam_search_decode_logits
 from .model import Encoder, CTCRecognizer, StarRecognizer
 from .resnet import FixupResNet, FixupBasicBlock
 from .xen import Vocabulary
 from . import symbol_tape
-
+from .rnnlm import LM
+from .transducer import transducer_forward_score
+from .ctc import ctc_reduce_mean
 
 console = Console()
 def print(*args, flush=False, **kwargs):
     console.log(*args, **kwargs)
 
 
 class Collator:
@@ -58,112 +60,164 @@
         match args.star_penalty:
             case None:
                 self.recognizer = CTCRecognizer(vocab_size=len(self.vocab)).to(args.device)
             case star_penalty:
                 self.recognizer = StarRecognizer(star_penalty=star_penalty,
                                                  vocab_size=len(self.vocab)).to(args.device)    
 
-        self.optimizer = torch.optim.Adam(chain(self.encoder.parameters(), self.recognizer.parameters()), lr=args.lr)
+        if args.lm:
+            lm_checkpoint = torch.load(args.lm, map_location=args.device)
+            self.lm_args = lm_checkpoint['args']
+            self.lm = LM(vocab_size=len(self.vocab),
+                         emb_dim=self.lm_args['rnn_size'],
+                         hidden_dim=self.lm_args['rnn_size'],
+                         num_layers=self.lm_args['num_layers'],
+                         dropout=self.lm_args['dropout']).to(args.device)
+            #self.lm.load_state_dict(lm_checkpoint['model'])
+
+            self.optimizer = torch.optim.Adam(chain(self.encoder.parameters(),
+                                                    self.recognizer.parameters(),
+                                                    self.lm.parameters()), lr=args.lr)
+        else:
+            self.lm_args, self.lm = None, None
+
+            self.optimizer = torch.optim.Adam(chain(self.encoder.parameters(),
+                                                    self.recognizer.parameters()), lr=args.lr)
         self.scaler = torch.cuda.amp.GradScaler()
 
     def load_state_dict(self, checkpoint):
         self.encoder.load_state_dict(checkpoint['encoder'])
         self.recognizer.load_state_dict(checkpoint['recognizer'])
         self.scaler.load_state_dict(checkpoint['scaler'])
         self.optimizer.load_state_dict(checkpoint['optimizer'])
         self.vocab.load_state_dict(checkpoint['vocab'])
+        if self.lm is not None:
+            print('loading transducer lm')
+            self.lm.load_state_dict(checkpoint['lm'])
 
     def make_state_dict(self, **extra):
         return {
             'encoder': self.encoder.state_dict(),
             'recognizer': self.recognizer.state_dict(),
             'scaler': self.scaler.state_dict(),
             'optimizer': self.optimizer.state_dict(),
             'vocab': self.vocab.state_dict(),
+            'lm_args': self.lm_args,
+            'lm': self.lm.state_dict() if self.lm is not None else None,
         } | extra
 
+    def forward(self, inputs, targets, input_lengths, target_lengths):
+        device = self.args.device
+
+        N, _, _ = inputs.shape
+        inputs = inputs.to(device) # (N, T, C)
+        targets = targets.to(device) # (N, U)
+        input_lengths = input_lengths.to(device) # (N,)
+        target_lengths = target_lengths.to(device) # (N,)
+
+        #print(inputs, targets) # works best with --batch-size 1
+
+        input_lengths = self.encoder.subsampled_lengths(input_lengths)
+
+        with torch.autocast(device_type='cuda', dtype=torch.float16):
+            outputs = self.encoder(inputs) # (N1, T, C)
+
+            if self.lm is not None:
+                #
+                # Output dependencies are controller by LM
+                #
+                hidden = self.lm.init_hidden(N)
+
+                # input needs to start with 0
+                lm_targets = torch.cat([targets.new_zeros((N, 1)), targets], dim=1) # (N, U1)
+
+                lm_outputs, _ = self.lm.forward_batch_first(lm_targets, hidden) # (N, U1, C)
+
+                outputs = self.recognizer.dropout(outputs)
+                outputs = self.recognizer.classifier(outputs) # (N, T, C)
+
+                joint = outputs[:, :, None, :] + lm_outputs[:, None, :, :] # (N, T, U1, C)
+                #joint = joint.log_softmax(dim=-1)
+
+                #loss = ctc_reduce_mean(transducer_forward_score(joint, targets, input_lengths, target_lengths), target_lengths)
+
+                from torchaudio.functional import rnnt_loss
+                loss = rnnt_loss(joint,
+                                    targets.to(torch.int32),
+                                    input_lengths.to(torch.int32),
+                                    target_lengths.to(torch.int32),
+                                    blank=0, reduction='mean', fused_log_softmax=True)
+            else:
+                #
+                # All outputs are independent
+                #
+                loss = self.recognizer(outputs, targets, input_lengths, target_lengths)
+
+        return loss, outputs
+
     def train_one_epoch(self, epoch, train_loader):
-        args, device = self.args, self.args.device
         encoder, recognizer, optimizer, scaler = self.encoder, self.recognizer, self.optimizer, self.scaler
 
         optimizer.zero_grad()
         encoder.train()
         recognizer.train()
 
         train_loss = 0.
         t0 = time.time()
         for i, (inputs, targets, input_lengths, target_lengths) in enumerate(train_loader):
-            inputs = inputs.to(device)
-            targets = targets.to(device)
-            input_lengths = input_lengths.to(device)
-            target_lengths = target_lengths.to(device)
-
-            #print(inputs, targets) # works best with --batch-size 1
-
-            input_lengths = encoder.subsampled_lengths(input_lengths)
-
-            with torch.autocast(device_type='cuda', dtype=torch.float16):
-                outputs = encoder(inputs)
-                loss = recognizer(outputs, targets, input_lengths, target_lengths)
+            loss, _ = self.forward(inputs, targets, input_lengths, target_lengths)
 
             if torch.isnan(loss):
                 print(f'[{epoch + 1}, {i + 1:5d}], loss is nan, skipping batch', flush=True)
                 scaler.update()
                 continue
 
             if torch.isinf(loss):
                 print(f'[{epoch + 1}, {i + 1:5d}], loss is inf, skipping batch, skipping scaler update', flush=True)
                 continue
 
             scaler.scale(loss).backward()
             scaler.unscale_(optimizer)
             grad_norm = torch.nn.utils.clip_grad_norm_(chain(encoder.parameters(), recognizer.parameters()), 0.1)
+            if self.lm:
+                grad_norm = 0.5*(grad_norm + torch.nn.utils.clip_grad_norm_(self.lm.parameters(), 0.1))
             if torch.isinf(grad_norm) or torch.isnan(grad_norm):
                 print(f'[{epoch + 1}, {i + 1:5d}], grad_norm is inf or nan, skipping batch', flush=True)
                 scaler.update()
                 optimizer.zero_grad(set_to_none=True)
                 continue
 
             scaler.step(optimizer)
             scaler.update()
             optimizer.zero_grad(set_to_none=True)
 
             train_loss += loss.item()
-            if i and i % args.log_interval == 0:
-                train_loss = train_loss / args.log_interval
+            if i and i % self.args.log_interval == 0:
+                train_loss = train_loss / self.args.log_interval
                 t1 = time.time()
                 print(f'[{epoch + 1}, {i + 1:5d}] time: {t1-t0:.3f} loss: {train_loss:.3f} grad_norm: {grad_norm:.3f}', flush=True)
                 wandb.log({'train/loss': train_loss, 'train/grad_norm': grad_norm})
                 t0 = t1
+                train_loss = 0.
 
     @torch.inference_mode()
     def evaluate(self, epoch, valid_loader):
-        device = self.args.device
         encoder, recognizer, vocabulary = self.encoder, self.recognizer, self.vocab
 
         valid_loss = 0.
         lers = []
 
         encoder.eval()
         recognizer.eval()
         for i, (inputs, targets, input_lengths, target_lengths) in enumerate(valid_loader):
-            inputs = inputs.to(device)
-            targets = targets.to(device)
-            input_lengths = input_lengths.to(device)
-            target_lengths = target_lengths.to(device)
-
-            input_lengths = encoder.subsampled_lengths(input_lengths)
-
-            outputs = encoder(inputs)
-            loss = recognizer(outputs, targets, input_lengths, target_lengths)
+            loss, outputs = self.forward(inputs, targets, input_lengths, target_lengths)
 
             valid_loss += loss.item()
 
             if i < 10:
-                outputs = recognizer.log_probs(outputs)
                 for ref, ref_len, seq, hyp_len in zip(targets, target_lengths, outputs, input_lengths):
                     seq = seq[:hyp_len].cpu()
                     ref = ref[:ref_len].cpu().tolist()
                     #print('greedy', seq.argmax(dim=-1).tolist())
                     decoded = ctc_beam_search_decode_logits(seq)
                     hyp1 = vocabulary.decode(filter(None, decoded[0][0]))
                     ref1 = vocabulary.decode(ref)
@@ -215,16 +269,16 @@
     parser.add_argument('--lr', type=float, default=3e-4, help="Adam learning rate")
     parser.add_argument('--train', type=str, help="Datasets to train on, comma separated")
     parser.add_argument('--eval', type=str, default='dev-clean', help="Datasets to evaluate on, comma separated")
     parser.add_argument('--encoder', type=str, default='lstm', choices=['lstm', 'r9'], help="Encoder to use: unidirectional LSTM or ResNet")
     parser.add_argument('--compile', action='store_true', help="torch.compile the model (produces incompatible checkpoints)")
     parser.add_argument('--star-penalty', type=float, default=None, help="Star penalty for Star CTC. If None, train with regular CTC")
     parser.add_argument('--num-workers', type=int, default=32, help="Number of workers for data loading")
-    parser.add_argument('--glottal-closures', action='store_true', help="Add glotal closures to the vocabulary")
     parser.add_argument('--vocab', type=str, default='bytes', choices=['bytes', 'cmu', 'xen'], help="Vocabulary to use: raw bytes, CMUdict, Xen (CMUdict + glottal closures)")
+    parser.add_argument('--lm', type=Path, help="Path to language model checkpoint trained with hal.")
     return parser
 
 
 def main():
     args = make_parser().parse_args()
     print(args)
```

### Comparing `haloop-0.0.6/ha/model.py` & `haloop-0.0.7/ha/model.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.6/ha/resnet.py` & `haloop-0.0.7/ha/resnet.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.6/ha/rnnlm.py` & `haloop-0.0.7/ha/rnnlm.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.6/ha/scan.py` & `haloop-0.0.7/ha/scan.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.6/ha/star.py` & `haloop-0.0.7/ha/star.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.6/ha/symbol_tape.py` & `haloop-0.0.7/ha/symbol_tape.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.6/ha/transducer.py` & `haloop-0.0.7/ha/transducer.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.6/ha/xen.py` & `haloop-0.0.7/ha/xen.py`

 * *Files identical despite different names*

### Comparing `haloop-0.0.6/LICENSE` & `haloop-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `haloop-0.0.6/pyproject.toml` & `haloop-0.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 Documentation = "https://github.com/proger/ha1#readme"
 Issues = "https://github.com/proger/ha1/issues"
 Source = "https://github.com/proger/ha1"
 
 [project.scripts]
 hac = "ha.loop:main"
 hal = "ha.rnnlm:main"
+hat = "ha.attention:main"
 
 [tool.hatch.version]
 path = "ha/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
```

