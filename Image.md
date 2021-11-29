```
if (flag)
            {
                File.Copy(ofd.FileName,_imgSource, true);
                _currentAgent.Logo = $"\\agents\\{ofd.SafeFileName}";
            }
```
