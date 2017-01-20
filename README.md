# Xiami_To_Spotify


## introduction:
This is a project in purpose to enable user to transfer music from [Xiami](http://www.xiami.com) to [Spotify](https://www.spotify.com/us/).

The music get from **Xiami -> my music 我的音乐 -> Spotify -> playlist -> From_Xiami (we create for you)**

## Step:

####    Xiami:
Knowing your
- [ ] username
- [ ] password

####     Spotify:
- [ ] username (if your username if from facebook, or have space between, this app may not work for you, change it to one word)

![image](https://drive.google.com/open?id=0B1ClAnzq00KsQzNESlgxcGhMRDA)
- [ ] [Spotify Application Sign in with your spotify account](https://developer.spotify.com/my-applications/)
![Alt text](/relative/path/to/img.jpg?raw=true "Optional Title")
- [ ] Create Application (name whatever you want, I personally recommand 'Xiami_connection' for example)
- [ ] after you successfully create an application, you will see Client_id and Client_Secret, keep these two information

- [ ] You will also see Redirect URIs after it, in there Paste [http://github.com/zhang435/Xiami_To_Spotify/](http://github.com/zhang435/Xiami_To_Spotify/) and click add
    Now download the [code](https://github.com/zhang435/Xiami_To_Spotify/archive/master.zip). remember click save at the button!

- [ ] At the bottom at main.py, replace information with you own information.
```python
if __name__ == '__main__':
move = Xiami_to_Spotify('XIAMI_USERNAME','XIAMI_PASSWORD','SPOTIFY_USERNAME','CLIENT_ID','CLIENT_CECRET')
move.start()
```
- [ ] go to terminal (if you use window,make sure you install python2 first [install](http://stackoverflow.com/questions/21372637/installing-python-2-7-on-windows-8), while if you are mac user, lucky you , python2 come with mac)
- [ ] in terminal(in window, it is command line?)return
`pip install request`
`pip install spotipy`

- [ ] in terminal run `python main.py`


## Reference:
[Spotify API](https://developer.spotify.com/web-api/)

[Spotipy Python Package](https://github.com/plamere/spotipy)

[spotipy Documentation](http://spotipy.readthedocs.io/en/latest/)

[urllib using](https://github.com/liyuntao/SignXiami)


## PROBLEM:
xiami is poplar used in Chinese market, it is not surprise that there are many some that user have is in chinese name

> Spotify does not have that a few Chinese song, but there most of them can be found "manually"

> I blame this problem on the developer who collect song resouces, for example it has name for both Simplifed Chinese and traditional Chinese. but if you search with only simplfied , you may not find the song even it is actully there, same for traditional chinese. AND, some chinese singer are named in english....which is impossibel to search correctly

> for me 900 are enable to pass 550, still need improve :)
