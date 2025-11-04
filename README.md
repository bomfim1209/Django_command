# Django_command
<p>Lista dos comandos mais utilizados e comandos úteis no dia a dia.</p>

# -----------
<h2>Comandos Para auxiliar na hora de migrar as tabelas</h2>
<p><b>python manage.py showmigrations</b> --> Lista todas as migrações que já foram feitas e as pendentes no banco de dados.</p>
<p><b>python manage.py migrate --fake zero</b> --> Se o banco está totalmente desalinhado e você quer zerar tudo e recriar as tabelas do zero, marca todas as migrations como não aplicadas, sem apagar tabelas.</p>
<p><b>python manage.py migrate --run-syncdb</b> --> Se você adicionou apps antigas (sem arquivos de migrations) e quer forçar a criação das tabelas, útil quando você está integrando código legado.</p>


<p><b>find caminho-pasta -type f ! -name '__init__.py' -delete</b> --> Exclui todos os arquivos com exceção daquele indicado.</p>
