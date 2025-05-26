# gensyn-full-guide
🚀Credit: Gensyn Node Guide is created by ZUN, I have adjusted Acc to own style so that my community can easily join the Gensyn testnet.

#install dependencies and go ahead

<pre> sudo apt update && sudo apt install -y python3 python3-venv python3-pip curl wget screen git lsof && curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add - && echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list && sudo apt update && sudo apt install -y yarn  </pre>

<pre> curl -sSL https://raw.githubusercontent.com/zunxbt/installation/main/node.sh | bash   </pre>

<pre> cd $HOME && [ -d rl-swarm ] && rm -rf rl-swarm; git clone https://github.com/zunxbt/rl-swarm.git && cd rl-swarm   </pre>

<pre> cd $home  </pre>

<pre> sudo apt install nano </pre>

<pre> cd $HOME/rl-swarm/hivemind_exp/configs/mac/ </pre>
<pre> ls   </pre>
then it will show a file copy the file name 
then 
	<pre> nano ....file-name.... </pre>
. Now replace below things in file

(A) torch_dtype = float32
(B) bf16 : false
(C) tf32 : false
(D) gradient_checkpointing: false
(E)per_device_train_batch_size: 2
(F)Training arguments : max_steps: 200
 ⚡After doing this press Ctrl+X then Y then enter
<pre> \```Screen -S gensyn   </pre>
<pre> cd $HOME/rl-swarm/  </pre>
<pre> python3 -m venv .venv && . .venv/bin/activate && ./run_rl_swarm.sh </pre>

then select model A
and then select 32 or 7 
then N
to get private keys and data
<pre> cat ~/rl-swarm/modal-login/temp-data/userApiKey.json  </pre>
 <pre> cat ~/rl-swarm/modal-login/temp-data/userData.json </pre>

 you will get the swarm.pem file in sftp in termius if you are using google cloud
go for run
Thanks
