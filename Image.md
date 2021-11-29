```
if (flag)
            {
                File.Copy(ofd.FileName,_imgSource, true);
                _currentAgent.Logo = $"\\agents\\{ofd.SafeFileName}";
            }
```
```
public string ImageAgent
        {
            get
            {
                string imageSource = "";
                string imageNullValue = "";
                string dictionary = Environment.CurrentDirectory;

                if((Logo == null ) || (Logo == ""))
                {
                    imageNullValue = "Resources\\picture.png";
                    imageSource = dictionary.Replace("bin\\Debug", "") + imageNullValue;
                }
                else
                {
                    imageNullValue = Logo;
                    imageSource = dictionary.Replace("bin\\Debug", "") + imageNullValue;
                }

                return imageSource;
            }
        }
        ```

<Image
  Width="100"
 Source="{Binding ImageAgent}">

</Image>


