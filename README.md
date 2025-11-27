# Django_command
<p>Lista dos comandos mais utilizados e comandos úteis no dia a dia.</p>

# -----------
<h2>Comandos Para auxiliar na hora de migrar as tabelas</h2>
<p><b>python manage.py showmigrations</b> --> Lista todas as migrações que já foram feitas e as pendentes no banco de dados.</p>
<p><b>python manage.py migrate --fake zero</b> --> Se o banco está totalmente desalinhado e você quer zerar tudo e recriar as tabelas do zero, marca todas as migrations como não aplicadas, sem apagar tabelas.</p>
<p><b>python manage.py migrate --run-syncdb</b> --> Se você adicionou apps antigas (sem arquivos de migrations) e quer forçar a criação das tabelas, útil quando você está integrando código legado.</p>


<p><b>find caminho-pasta -type f ! -name 'come-arquvo' -delete</b> --> Exclui todos os arquivos com exceção daquele indicado.</p>

# -----------
<h2>Criando uma nova DJANGO_SECRET_KEY</h2>
<p>Execute os seguintes comandos no seu shell.</p>
<ol>
  <li>python</li>
  <li>from django.core.management.utils import get_random_secret_key</li>
  <li>print(get_random_secret_key())</li>
</ol>
<p>O codigo exibido é a nova chave gerada pelo seu Django. Copie e salve para não esquecer.</p>
<p>Para sair do terminal do python basta executar o comando CTRL + Z(o "z" tem que estar em caixa alta).</p>

# -----------
<h2>Criando Super Usuário</h2>
<p><b>python manage.py createsuperuser</b></p>

# -----------
<h2>Coletando arquivos Estaticos</h2>
<ol>
  <li>No settings.py, defina o item STATIC_ROOT.</li>
  <li>STATIC_ROOT = os.path.join(BASE_DIR, 'staticfiles')</li>
</ol>
<p>Depois no seu terminal execute o seguinte comando:</p>
<p><b>python manage.py collectstatic</b></p>
