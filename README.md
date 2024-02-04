# ShareApp

<p align="center"><a href="https://github.com/AbhiTheModder"><img title="Abhi The MØÐÐĒR" src="https://github-readme-stats.vercel.app/api?username=AbhiTheModder&show_icons=true&include_all_commits=true&theme=chartreuse-dark&cache_seconds=3200"></a>
</p>

<p align="center">
<a href="https://github.com/AbhiTheModder"><img title="GitHub" src="https://img.shields.io/badge/Abhi-TheModder-brightgreen?style=for-the-badge&logo=github"></a>
<a href="https://www.youtube.com/channel/UCtBILuQgvXHPfvOUdcmMS2Q"><img title="YouTube" src="https://img.shields.io/badge/YouTube-Abhi The MØÐÐĒR-red?style=for-the-badge&logo=Youtube"></a>
</p>

## Create a new drawable resource file and add these lines

        <shape

    xmlns:android="http://schemas.android.com/apk/res/android">
    <stroke android:color="@color/black"
    android:width="2dp"/>
    <solid
        android:color="#00FFFFFF"/>

     </shape>


## In activity_main.xml file add these lines but firstly add your desired share image in drawable file  

     <RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".detils"
    android:orientation="vertical">

    <ImageButton
        android:id="@+id/tg_btn"
        android:layout_width="113dp"
        android:layout_height="105dp"
        android:layout_centerHorizontal="true"
        android:layout_marginLeft="150dp"
        android:layout_marginTop="100dp"
        android:background="@drawable/back"
        android:src="@drawable/ic_join" />

    <ImageButton
        android:id="@+id/fb_btn"
        android:layout_width="100dp"
        android:layout_height="110dp"
        android:layout_below="@+id/tg_btn"
        android:layout_centerHorizontal="true"
        android:layout_marginLeft="150dp"
        android:layout_marginTop="49dp"
        android:background="@drawable/back"
        android:src="@drawable/fb" />


     </RelativeLayout>

## Now add these in MainActivity.java


    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        findViewById(R.id.tg_btn).setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                clicked_btn("https://telegram.org");
            }
        });

        findViewById(R.id.fb_btn).setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                clicked_btn("https://www.facebook.com");
            }
        });

    }

    public void clicked_btn(String url)
    {
        Intent intent=new Intent(Intent.ACTION_VIEW);
        intent.setData(Uri.parse(url));
        startActivity(intent);
    }

    }
# To Contact Me 
## Vist links below 
<p align="center">
<a href="https://t.me/joinchat/xP-wW-A5mIBmMjY1"><img title="Telegram" src="https://img.shields.io/badge/Telegram-black?style=for-the-badge&logo=Telegram"></a>
<a href="https://t.me/QbtaumaiBot"><img title="Telegram Bot" src="https://img.shields.io/badge/Telegram-bot-black?style=for-the-badge&logo=Telegram_bot"></a>
