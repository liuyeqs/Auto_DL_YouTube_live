## YouTubeライブを自動ダウンロード

### 1. プログラムを実行する前に、
    必要なパッケージをインストールください。
    pip install -U -r requirements.txt


### 2. プログラムの入力パラメータ:
  -h, --help      show this help message and exit  
  --url           https://www.youtube.com/*****  
  --CCTV          CCTVカメラの名前/場所  
  --chunks        ビデオの長さ  
  --step          10フレーム毎で画像作成  
  --ext           画像ファイル形式  
  --dir_videos    ビデオの保存場所  
  --dir_frames    フレーム・画像の保存場所  
  --dontsv_frames   フレーム・画像を作成するか否か  
  --save_videos   ビデオを保存するか否か  

####  コマンド入力例：

    1) フレーム・画像作成、ビデオ保存しない
    python get_yt_live.py --url https://www.youtube.com/*****

    2) フレーム・画像作成、ビデオ保存
    python get_yt_live.py --url https://www.youtube.com/***** --save_videos

    3) フレーム・画像作成しない、ビデオ保存
    python get_yt_live.py --url https://www.youtube.com/***** --dontsv_frames --save_videos

    4) 個人の需要により
    python get_yt_live.py --url https://www.youtube.com/***** --CCTV Kyushu --chunks 100 --step 15 --dir_videos C:/Users/ユーザー名/Desktop/output --dir_frames C:/Users/ユーザー名/Desktop/frames
