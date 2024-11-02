1. 最初にテストコードをcloneしてきます。
```
git clone https://github.com/hyptpc/tpc_ana_example.git
```

2. コードの場所に移動します
```
cd tpc_ana_example
```

3. root fileに直したデータは`/hsm/had/sks/Users/sryuta/TOHOKU2024Jan_root`に置いてあります。アクセスしやすいように作業する場所にシンボリックリンクを作ります。
```
ln -s /hsm/had/sks/Users/sryuta/TOHOKU2024Jan_root data
```

4. ROOTを起動して、`simple_check_track.C`を読み込みます。マクロを読み込んだ時にCanvasが出てくるはずです。
```
root
.L simple_check_track.C
```

![image](https://github.com/user-attachments/assets/48e50d32-e6ea-4585-907f-c238de3cb1e4)

5. `set_path("root_file_path")`のようにしてroot fileのパスを設定します。
![image](https://github.com/user-attachments/assets/45b5751a-c4fc-4416-a75b-80b249d6c5c0)

6. `event()`を実行すると、ランダムにHypTPCで測定したデータが確認できます。`event()`を繰り返し実行すれば別のイベントも見れます。特定のイベントを見たい場合は`event(evnum)`とすればOKです。

![image](https://github.com/user-attachments/assets/564fd6b3-1258-478d-9a60-0acd5dc03b14)

