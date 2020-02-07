MusicEngine
===========

**概要:**  
音楽を再生するオブジェクトにテンポや拍子を指定する事で  
音楽のタイミングを取得したりクオンタイズさせたり  
音楽に合わせた演出を簡単に作れるようになります。  

また、複数のセクションや複数のトラックを追加して  
小節に合わせた横の遷移や  
クロスフェードによる縦の遷移を  
関数一つで簡単に実行できます。  

Unity単体での再生と、CRI ADX2を使った再生に対応しています。

**利用方法:**  
MusicEngineフォルダごとプロジェクトに追加してください。  

Unity単体で利用する場合はMusicUnityコンポーネントを追加し、Sectionsの中にAudioClipを追加してください。  
（AudioSourceコンポーネントは再生時に内部で自動的に生成されます）  

ADX2を利用する場合は、MusicADX2.csの #define ADX2 を有効にした上で、  
MusicADX2コンポーネントをCriAtomSourceコンポーネントと同じオブジェクトに追加してください。

何か使い方や変数の意味がわからなかったり、使いにくかったりする場合は  
@geekdrums までご連絡いただけると、今後の改善の参考にさせていただきます。  


**Abstract:**  
You can get musical timing information with Unity or CRI ADX2.  

And you can also use interactive music functions such as Horizontal Resequencing and Vertical Remixing.


**How To Use:**  
Add MusicEngine folder to your Unity project.

Use MusicUnity component if you don't use any other audio middleware.  
Add MusicUnity component and set AudioClips into Sections property.
(AudioSource component will be automatically instantiated inside this MusicEngine.)

If you use CRI ADX2 (audio middleware),  enable #ADX2 in MusicADX2.cs.  
Add MusicADX2 component to the same gameObject with CriAtomSource component.

If you have any questions or suggestions, please let me (@geekdrums) know.  
