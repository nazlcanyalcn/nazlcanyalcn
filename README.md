- 👋 Hi, I’m @nazlcanyalcn
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
nazlcanyalcn/nazlcanyalcn is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
"""
MIT License

Copyright (c) 2020-2024 EntySec

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
"""

from setuptools import setup, find_packages

setup(name='hatsploit',
      version='5.0.0',
      description='Modular penetration testing platform that enables you to write, test, and execute exploit code.',
      url='https://github.com/EntySec/HatSploit',
      author='EntySec',
      author_email='entysec@gmail.com',
      license='MIT',
      python_requires='>=3.7.0',
      packages=find_packages(),
      include_package_data=True,
      entry_points={
          "console_scripts": [
              "hsf = hatsploit:hsf_cli",
              "hsfgen = hatsploit:gen_cli"
          ]
      },
      install_requires=[
          'impacket',
          'packaging',
          'pyyaml',
          'flask',
          'flask_cors',
          'flask_restful',
          'pyngrok',
          'jsonrpclib',
          'hatasm @ git+https://github.com/EntySec/HatAsm',
          'pex @ git+https://github.com/EntySec/Pex',
          'colorscript @ git+https://github.com/EntySec/ColorScript',
          'pwny @ git+https://github.com/EntySec/Pwny',
      ],
      zip_safe=False,
      )
